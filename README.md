# Hono Alibaba Cloud FC3 Adapter

[![Build](https://github.com/rwv/hono-alibaba-cloud-fc3-adapter/actions/workflows/build.yml/badge.svg)](https://github.com/rwv/hono-alibaba-cloud-fc3-adapter/actions/workflows/build.yml)
[![NPM Version](https://img.shields.io/npm/v/hono-alibaba-cloud-fc3-adapter)](https://www.npmjs.com/package/hono-alibaba-cloud-fc3-adapter)
![GitHub License](https://img.shields.io/github/license/rwv/hono-alibaba-cloud-fc3-adapter)

An adapter for using [Hono](https://hono.dev) with [Alibaba Cloud Function Compute 3.0](https://www.alibabacloud.com/help/en/functioncompute/fc-3-0).

一个用于在[阿里云函数计算 FC 3.0](https://help.aliyun.com/zh/functioncompute/fc-3-0/) 中使用 [Hono](https://hono.dev) 的适配器。

## Installation

```bash
npm install hono-alibaba-cloud-fc3-adapter
```

## Usage

```typescript
import { Hono } from "hono";
import { handle } from "hono-alibaba-cloud-fc3-adapter";

const app = new Hono();

app.get("/", (c) => c.text("Hello Hono!"));

export const handler = handle(app);
```

For more details, check out [Alibaba Cloud Function Compute - Hono](https://hono.dev/docs/getting-started/ali-function-compute).
