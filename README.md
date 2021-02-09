### MiTour

**Changed and improved functions.**

Added function `skipNotExistNode()` for steps.

Skips the step if the element is not found in the DOM tree.
If the function is not specified step, then go to the next.

```js
const tourConfig = [
  {
    skipNotExistNode: ({current, goTo}) => {
        console.log(`skip ${current}`);
    },
    selector: '[data-tut="reactour__iso"]',
    content:
      "Ok, let's start with the name of the Tour that is about to begin.",
    actionBefore: async () => {
      await timeout(5000)
      console.log('Hola!')
    },
  }
]
```


This is a fork of this project
https://github.com/elrumordelaluz/reactour

