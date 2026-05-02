---
type: page
title: Run Code Technical Guide
seoTitle: Run Code Technical Guide
seoDescription: This guide explains the Run Code Action, a tool for executing JavaScript in workflows to process data and generate outputs. It includes setup instructions, usage details, debugging tips, examples, and known limitations.
slug: run-code-technical-guide
order: 24
status: published
---


# Run Code Technical Guide

This guide explains the [Run Code Action](/react-flow/run-code), a tool for executing JavaScript in workflows to process data and generate outputs. It includes setup instructions, usage details, debugging tips, examples, and known limitations.

## Runtime Environment & System APIs

The following are key runtime environment variables available during execution for managing data, interacting with external sources, and looping through items.

<table class="csh-markdown csh-markdown-table"><colgroup><col><col></colgroup><tbody><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">Name</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">Description</strong></b><span></span></p></td></tr><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">$graphql</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span>Executes </span><code spellcheck="false"><span class="csh-markdown csh-markdown-code csh-markdown-code-inline csh-font-code-regular">GraphQL</span></code><span> queries or mutations, used to retrieve, create, or update data in your </span><code spellcheck="false"><span class="csh-markdown csh-markdown-code csh-markdown-code-inline csh-font-code-regular">Shopify</span></code><span> store.</span></p></td></tr><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">$context</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span>A context object that provides access to runtime variables available for use within the workflow.</span></p></td></tr><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">$context.event</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span>A context object that contains variables passed from the </span><code spellcheck="false"><span class="csh-markdown csh-markdown-code csh-markdown-code-inline csh-font-code-regular">trigger</span></code><span> that started the workflow.</span></p></td></tr><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">$context.fetchItem</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span>A context object that provides access to variables within the current iteration of a </span><code spellcheck="false"><span class="csh-markdown csh-markdown-code csh-markdown-code-inline csh-font-code-regular">fetch</span></code><span> loop.</span></p></td></tr><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">$context.forEachItem</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span>A context object that provides access to variables within the current iteration of a </span><code spellcheck="false"><span class="csh-markdown csh-markdown-code csh-markdown-code-inline csh-font-code-regular">forEach</span></code><span> loop.</span></p></td></tr></tbody></table>

The following system APIs are available in the runtime environment for making HTTP requests and logging information during execution.

<table class="csh-markdown csh-markdown-table"><colgroup><col><col></colgroup><tbody><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">Name</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">Description</strong></b><span></span></p></td></tr><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">fetch</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span>Standard </span><code spellcheck="false"><span class="csh-markdown csh-markdown-code csh-markdown-code-inline csh-font-code-regular">fetch</span></code><span> function for making HTTP requests within the runtime environment.</span></p></td></tr><tr class="csh-markdown csh-markdown-table-row"><td class="csh-markdown csh-markdown-table-cell"><p><span></span><b><strong style="white-space:pre-wrap" class="csh-markdown csh-markdown-bold csh-font-sans-medium">console.log</strong></b><span></span></p></td><td class="csh-markdown csh-markdown-table-cell"><p><span>Standard logging function to output messages for debugging purposes during execution.</span></p></td></tr></tbody></table>

## GraphQL Service ($graphql)

The `$graphql` service is a powerful runtime utility that simplifies interactions with the Shopify Admin GraphQL API. It provides a clean, structured way to execute queries and mutations, abstracting away complex request handling while maintaining flexibility.

Below are practical examples of data querying and modification:

Fetches a list of recently updated orders with flexible filters:

(async () => {  
const { data } = await $graphql({  
query: \`query GetOrders($query: String!, $first: Int!) {  
orders(first: $first, query: $query) {  
nodes { id name updatedAt }  
}  
}\` ,  
variables: {  
first: 10,  
query: "updated\_at:>2025-04-01",  
},  
});

return {  
orders: data?. orders?. nodes ?? \[\],  
}  
})();

Manages customer tags to organize profiles for segmentation and targeting:

(async () => {  
const { data } = await $graphql({  
query: \`mutation($id: ID!, $tags: \[String!\]!) {  
tagsAdd(id: $id, tags: $tags) {  
node { id ... on Customer { tags } }  
userErrors { message }  
}  
}\`,  
variables: {  
id: $context.event.customer.admin\_graphql\_api\_id,  
tags: \["vip", "loyal"\],  
},  
});

return {  
tags: data?.tagsAdd?.node?.tags ?? \[\],  
};  
})();

## Fetch (fetch)

The Fetch API lets you make `HTTP` requests to interact with external services, such as fetching or sending data using methods like `GET`, `POST`, `PUT`, and `DELETE`. In this environment, the response data is already parsed and available in `response.data`, so you can use it directly without extra steps. The API works asynchronously, returning a Promise.

Below are practical examples of making HTTP requests using fetch:

(async () => {  
try {  
const { data } = await fetch(  
"[https://jsonplaceholder.typicode.com/posts/1](https://jsonplaceholder.typicode.com/posts/1)"  
);

      return {  
         post: data,  
      };  
    

} catch (err) {  
console.error(\`Error message: ${err?.message}\`);  
}  
})();

Sends JSON data to an external API endpoint.

(async () => {  
try {  
const { data } = await fetch("[https://jsonplaceholder.typicode.com/posts](https://jsonplaceholder.typicode.com/posts)", {  
method: "POST",  
headers: {"Content-Type": "application/json" },  
body: JSON.stringify({  
title:"Sample Post",  
body:"This is a test post.",  
userId: 1,  
}),  
});

return {  
post: data,  
};  
} catch (err) {  
console.error(\`Error message:${err?.message}\`);  
}  
})();

## Console.log

The `console.log` function outputs messages, variables, or data to the workflow's Server logs for debugging and monitoring code execution. Logs appear in the Server logs section of the workflow result interface, helping you track and diagnose issues efficiently. The following are valid examples:

console.log("Start"); // Start

const input = {  
order: { id: 1, items: \[{ name: "Book"}\] },  
};

console.log(input); // { order: { id: 1, items: \[ { name: 'Book' } \] } }

You can also use `console.warn` for warnings and `console.error` for errors to clearly distinguish and categorize output messages.

## Output data

The Run Code action allows you to return custom data as a result of its execution. To specify the structure and types of the returned data, use the Output field with GraphQL's `Schema Definition Language (SDL)`. The supported scalar types include `String`, `Int`, `Float`, and `Boolean`, which follow `SDL` conventions for marking fields as required, defining lists, or creating custom types.

The following example calculates the total value of a customer's five most recent orders and returns an object containing the customer's name and the calculated sum.

(async () => {  
const { data } = await $graphql({  
query: \`query GetCustomerOrders($id: ID!, $first: Int!, $sortKey: OrderSortKeys!, $reverse: Boolean!) {  
customer(id: $id) {  
displayName  
orders(first: $first, sortKey: $sortKey, reverse: $reverse) {  
nodes { totalPriceSet { shopMoney { amount }}}  
}  
}  
}\`,  
variables: {  
id: $context.event.admin\_graphql\_api\_id,  
first: 5,  
sortKey: "CREATED\_AT",  
reverse: true,  
},  
});

const orders = data?.customer?.orders?.nodes ?? \[\]  
const sum =orders.reduce(  
(total, { totalPriceSet }) =>  
total + parseFloat(totalPriceSet?.shopMoney?.amount ?? 0),  
0  
);

return {  
displayName: data?.customer?.displayName,  
sum,  
};  
})();

The data schema defined in the `Define output` field must exactly match the object returned by the action through `return`. Once the properties are specified in the `Output` type, they become accessible in workflow steps as variables and conditions. Comments are optional, but will be used to describe the data in the workflow UI.

"The output of Run Code"  
type Output {  
"Full name of the customer"  
displayName: String  
"Total amount from the customer's last 5 orders"  
sum: Int  
}

## Limitations

The Run Code action has the following limitations:

*   The Run Code action supports `ECMA2020 JavaScript`. It does not support the `NodeJS` or `CommonJS APIs`, or importing modules.
*   `Console.log` does not output to the browser console.
*   Code cannot be longer than `50,000` characters.
*   Output data schema cannot be longer than `1,000` characters.
*   `Console.log` output is limited to a combined `2KB`.
*   Output data payload is limited to a combined `10KB`.
*   Total execution duration is limited to `70` seconds.
*   Memory usage is limited to `10MB`.
