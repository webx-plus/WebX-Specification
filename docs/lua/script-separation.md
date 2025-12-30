---
title: Script Separation
description: Lua script separation notice.
parent: Lua
nav_order: 3
---
# Lua Script Separation

In WebX multiple scripts don't share things like variables (similar to type="module" in normal HTML), this may cause some issues for sharing values.\
In the v2 API you can use the [global](v2/globals/global.md) table to share values between scripts.
