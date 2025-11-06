# 🚀 Deployment Guide for MERN Projects

## 🔹 Vercel JSON Config for Express Backend

```json
{
  "version": 2,
  "builds": [
    {
      "src": "server.js",
      "use": "@vercel/node",
      "config": {
        "includeFiles": [
          "dist/**"
        ]
      }
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "server.js"
    }
  ]
}



