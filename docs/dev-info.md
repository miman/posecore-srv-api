## How to generate and build the TypeScript API library

### 1. Install dependencies

```
npm install
```

### 2. Generate TypeScript client code from OpenAPI

```
npm run generate
```

This uses [openapi-generator-cli](https://openapi-generator.tech/docs/installation) to generate TypeScript code from `openapi.yaml` into the `src` folder.

### 3. Build the library

```
npm run build
```

This compiles the generated TypeScript code and bundles it as a reusable library in the `dist` folder.

### 4. Use in other projects

You can import the built library from the `dist` folder in other PoseCore sub-projects (such as `demo-app` or `client`).

---

**Note:**

- You can customize the OpenAPI generator options in the `package.json` script.
- Make sure to re-run `npm run generate` and `npm run build` after updating `openapi.yaml`.
