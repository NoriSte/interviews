
# First exercise

Find the longest common path

/home/humanitec/projects/readme.txt
/home/humanitec/projects/other/my-app.go
/home/humanitec/document/other/doc-gen.sh


# Second exercise

Write a function that converts an array of objects into a tree, where each object is nested in its parent object. a
If the parent property is null then that object should be the root node.
E.g., for the array:

```js
{id: 15, color: 'yellow' parent: null},
{id: 4, color: 'blue', parent: 8},
{id: 7, color: 'yellow', parent: 15},
{id: 8, color: 'red', parent: 5},
{id: 5, color: 'pink' parent: 7},
{id: 20, color: 'green', parent: 8}
```
you would create this tree object:
```js
{
  id: 15,
  color: 'yellow',
  parent: null,
  children: [
    {
      id: 7,
      color: 'yellow',
      parent: 15,
      children: [
        {
          id: 5,
          color: 'pink',
          parent: 7,
          children: [
            {
              id: 8,
              color: 'red',
              parent: 5,
              children: [
                { id: 20, color: 'green', parent: 8 },
                { id: 4, color: 'blue' },
              ],
              parent: 8,
            },
          ],
        },
      ],
    },
  ],
}

```
