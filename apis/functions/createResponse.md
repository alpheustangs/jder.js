[@jderjs/core](../README.md) / createResponse

# Function: createResponse()

```ts
function createResponse<D>(options?): Response;
```

Defined in: [index.ts:73](https://github.com/jder-std/core.js/blob/8f752d1679b827b4deb2cd21184bd81491ea8d2c/package/src/response/index.ts#L73)

Create a response.

### Examples

Example for creating a basic response:

```ts
import { createResponse } from "@jderjs/core";

const route = (): Response => {
    return createResponse();
};
```

Example for creating a response with status, headers, and body:

```ts
import { createResponse } from "@jderjs/core";

const route = (): Response => {
    return createResponse({
        status: 404,
        headers: [
            ["Content-Type", "text/plain"],
        ],
        body: "Not Found",
    });
};
```

## Type Parameters

### D

`D` *extends* `BodyInit` = `BodyInit`

## Parameters

### options?

[`CreateResponseOptions`](../type-aliases/CreateResponseOptions.md)\<`D`\>

## Returns

`Response`
