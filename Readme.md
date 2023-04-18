## Frontend Enginner Assignment 

# React Componet Code

### Here we have 2 file 
- [GivenCode.js](./GivenCode.js) (Code provided by SteelEye)
- [ModifiedCode.js](./ModifiedCode.js) (Modifed Code)

#### Q). What List Component Does ?

> **List Component** displays a list of items, it has two sub-components 
> - **WrappedSingleListitem** - for rendering individual list item and 
> - **WrappedListCompont**, - for rendering the whole list of items. <br><br>
> When any user clicks on a list item, the **handleClick** function is called with the item's index as an argument, which updates the selectedIndex state variable.<br><br>
> List component exports WrappedListComponent as a memoized component for improved performance.
> In other words we can say List component provides a reusable and flexible way to display a list of items with the ability to select and highlight individual items.

#### Q). What problem / warnings are there with code ?

>Following are the problems with the given code :
> - In **WrappedSingleListItem**, the **isSelected** prop is not being passed correctly.
> - In **WrappedSingleListItem**, the **onClickHandler** function should be wrapped in an arrow function to avoid calling the function during the rendering process.
> - In **WrappedListComponent**, the **handleClick** function should be defined outside of the component to prevent it from being recreated on every render.
> - In **WrappedListComponent**, the **items** prop type is not defined correctly. 
> - In **WrappedListComponent**, the useState hook is not used correctly.
> - In **WrappedListComponent**, the default value for items should be an empty array instead of null.

> Warraing we get when we run this code is :
```
Warning: Failed prop type: The prop isSelected is marked as required in SingleListItem, but its value is undefined.
```

### Fixed and Optimized Code is in [ModifiedCode.js](ModifiedCode.js) file