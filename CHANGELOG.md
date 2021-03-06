## 0.3.3

*   Automatically generate IDisplayName when not explicitly defined.

## 0.3.2

*   Fix DOM functions to properly handle non-literal nested attributes

## 0.3.0

*   Upgrade to Om 0.7.1
*   BREAKING: components with mixins generate React descriptor with "$descriptor"
    suffix rather than a React constructor with a "$ctor" suffix.

## 0.2.3

*   Change non-essential dependencies to be transient to avoid conflicting with
    user supplied dependencies.

## 0.2.2

*   Upgrade dependency: schema 0.2.4
*   Upgrade dependency: plumbing 0.3.2

## 0.2.1

*   Add `om-tools.mixin` namespace for defining Om mixins
*   Add `:mixin` option to `defcomponent`/`defcomponentk` macro to generate
    React component constructor with mixins configured.
*   Fixes `om-tools.dom` unparsed attribute values for maps.
*   Fixes `om-tools.dom` unwanted camelCasing of data-* and aria-* attributes.

## 0.2.0

*   Rename `defcomponent` macro to `defcomponentk` to indicate it uses
    `fnk`-style syntax and define `defcomponent` macro that uses normal
    `defn`-style arguments.
*   Add `om.core/set-state?!` function
*   Add `om.dom/class-set` function
*   Add `:shared` key option to `defcomponentk` for accessing shared
    Om data from `om.core/get-shared`.
*   Optimize `defcomponentk` macro to not create state proxy or shared
    data unless it is used.

## 0.1.1

*   Fix the need to use `#js` reader macro on :style attributes
