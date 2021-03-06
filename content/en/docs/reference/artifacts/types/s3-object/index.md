---
title: "S3 Object"
linkTitle: "S3 Object"
description: S3 object artifacts are references to objects stored in S3 buckets.
---

These artifacts are generally consumed by stages that read configuration from text files, such as a
Deploy Manifest or AWS Deploy stage.

## Fields

| Field | Explanation |
|-|-----------|
| `type` | Always `s3/object`. |
| `name` | Name/Path of the object. |
| `reference` | Name/Path of the object. |
| `location` | The region where your bucket was created |

## Example

```js
{
  "type": "s3/object",
  "name": "s3://bucket/file.json",
  "reference": "s3://bucket/file.json",
  "location": "us-east-1"
}
```
