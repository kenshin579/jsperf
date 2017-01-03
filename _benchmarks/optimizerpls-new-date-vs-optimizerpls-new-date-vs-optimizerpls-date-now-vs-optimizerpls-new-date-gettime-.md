---
title: optimizerPls = new Date(); vs optimizerPls = +new Date(); vs optimizerPls = Date.now(); vs optimizerPls = (new Date).getTime();
setup: |
  var optimizerPls = null;
tests:
  -
    name: new Date();
    code: |
      optimizerPls = new Date();
  -
    name: +new Date();
    code: |
      optimizerPls = +new Date();
  -
    name: Date.now();
    code: |
      optimizerPls = Date.now();
  -
    name: (new Date).getTime();
    code: |
     optimizerPls = (new Date).getTime();
---

