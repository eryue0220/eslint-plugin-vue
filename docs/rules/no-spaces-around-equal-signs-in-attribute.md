---
pageClass: rule-details
sidebarDepth: 0
title: vue/no-spaces-around-equal-signs-in-attribute
description: disallow spaces around equal signs in attribute
since: v5.0.0
---

# vue/no-spaces-around-equal-signs-in-attribute

> disallow spaces around equal signs in attribute

- :gear: This rule is included in all of `"plugin:vue/strongly-recommended"`, `*.configs["flat/strongly-recommended"]`, `"plugin:vue/vue2-strongly-recommended"`, `*.configs["flat/vue2-strongly-recommended"]`, `"plugin:vue/recommended"`, `*.configs["flat/recommended"]`, `"plugin:vue/vue2-recommended"` and `*.configs["flat/vue2-recommended"]`.
- :wrench: The `--fix` option on the [command line](https://eslint.org/docs/user-guide/command-line-interface#fix-problems) can automatically fix some of the problems reported by this rule.

## :book: Rule Details

This rule disallow spaces around equal signs in attribute.

<eslint-code-block fix :rules="{'vue/no-spaces-around-equal-signs-in-attribute': ['error']}">

```vue
<template>
  <!-- ✗ BAD -->
  <div class = "item"></div>
  <!-- ✓ GOOD -->
  <div class="item"></div>
</template>
```

</eslint-code-block>

::: tip Info
HTML5 allows spaces around equal signs. But space-less is easier to read, and groups entities better together.
:::

## :wrench: Options

```json
{
  "vue/no-spaces-around-equal-signs-in-attribute": ["error"]
}
```

## :books: Further Reading

- [HTML5 Style Guide - W3Schools _Spaces and Equal Signs_](https://www.w3schools.com/html/html5_syntax.asp)

## :rocket: Version

This rule was introduced in eslint-plugin-vue v5.0.0

## :mag: Implementation

- [Rule source](https://github.com/vuejs/eslint-plugin-vue/blob/master/lib/rules/no-spaces-around-equal-signs-in-attribute.js)
- [Test source](https://github.com/vuejs/eslint-plugin-vue/blob/master/tests/lib/rules/no-spaces-around-equal-signs-in-attribute.js)
