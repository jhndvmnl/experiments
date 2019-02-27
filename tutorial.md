# Tutorials Dev

## BEM - [block]__[element]--[modifier]

```
<figure class="photo">
  <img class="photo__img" src="#">
  <figcaption class="photo__caption">
    <p class="photo__quote">
      Look at me!
    </p>
  </figcaption>
</figure>
```
### Namespace

-	 .l -: layouts
-	 .o-: objects
-  .c-: components
-  .js: JavaScript hooks
-  .is-|.has-: state classes
-  .u-: utility classes

---

## CSS Specificity

1. Inline styles - An inline style is attached directly to the element to be styled. 

    Example: ```<h1 style="color: #ffffff;">```.

2. IDs - An ID is a unique identifier for the page elements, such as `#navbar`.

3. Classes, attributes and pseudo-classes - This category includes `.classes` , `[attributes]` and pseudo-classes such as `:hover` , `:focus` etc.

4. Elements and pseudo-elements - This category includes element names and pseudo-elements, such as `h1` , `div` , `:before` and `:after`.


### Calculate Specificity

- 1000 for style attribute
- 100 for each ID
- 10 for each attribute, class or pseudo-class
- 1 for each element name or pseudo-element

### Rules

- Equal specificity: the latest rule counts
- Contextual selectors are more specific than a single element selector
- A class selector beats any number of element selectors
- The universal selector and inherited values have a specificity of 0 

---

## Semantic Versioning

0.0.1


### Patch Versions
- Rightmost number is a `patch`
- there are no functionality changes
- when you increase a new patch, you increase the rightmost number by 1. From 1, you increase it to 2, then to 3, and so on.

### Minor Versions
- The second number is called the `minor` version number.
- used when you release new functionality in your project
- when you increase the minor version, you also increase it by one. But `when you increase the minor version, you must reset the patch version to zero`.

### Major Versions
- The leftmost number is a `major` version.
- when you increase the major version, you tell people that there are `backward-incompatible changes`
- when you `increase the major version number, you reset both patch version and minor versions`.

### Pre-releases

If you want to create a pre-release (like an alpha or beta version), you can add `a -` , followed by the words `alpha` or `beta`.

There are no hard and fast rules for pre-releases, so you can name them anything you want. Usually, we use alpha or beta, followed by a number, like `alpha1`.

### Starting a project

Most people start projects with 0.1.0. When you’re ready to release the project to the public, you increase the version to 1.0.0.

---
