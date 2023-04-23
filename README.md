
# Steel-Eye Frontend Engineer Assignment








## Q 1 - Explain what the simple List component does.


Ans - The List component is a simple React component that renders a list of items using the SingleListItem component.

The component takes in an array of items as a prop, which is an array of objects that have a text property. If the items prop is not provided, it uses a default array of objects.

The List component maps over the items array and renders a SingleListItem component for each item in the list. The SingleListItem component takes in props such as text, index, isSelected, and onClickHandler. It renders an <li> element with the text of the item and a background color that depends on whether the item is selected or not.

The List component uses the useState hook to maintain the selected index state and initializes it to undefined. It also defines a handleClick function that updates the selected index state with the index of the clicked item.

Both the SingleListItem and ListComponent components are memoized using the memo HOC to optimize performance by preventing unnecessary re-renders when props do not change.

Overall, the List component is a simple, reusable component that renders a list of items with the ability to select a single item.



## Q 2 - What problems / warnings are there with code?


## Problem 1 : Syntactical Error

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/shapeof.png?raw=true)
## Problem 1 : Code

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/shapeof1.png?raw=true)
## Problem 1 : Fixed Code

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/shapeofans.png?raw=true)

- PropTypes. shape is used when describing an object whose keys are known ahead of time, and may represent different types.


## Problem 2 : Syntactical Error

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/mapnull.png?raw=true)
## Problem 2 : Syntactical Error

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/mapq.png?raw=true)
## Problem 2 : Fixed Code

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/mapans.png?raw=true)

- So, you can just switch the places of selectedIndex and setSelectedIndex as in useState setSelectedIndex is a function to change the state of selectedIndex and its syntax is like this.
- And we can also remove useEffect as it doesn't have any work. 




## Problem 3 : No Props or Data in items

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/3map.png?raw=true)
## Problem 3 : No data

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/3q.png?raw=true)
## Problem 3 : Fixed Code

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/3ans.png?raw=true)

- So, we can do 2 things 1st is take data as props or take the default data from items
- So i have taken data from the default props to make things simple in this components.





## Problem 4 : Unique "key" in map

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/4.key.png?raw=true)
## Problem 4 : There was no unique "key" in this section

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/4.ans.png?raw=true)


- The main purpose of keys is to help React differentiate and distinguish elements from each other, increasing its performance when diffing between the virtual and real DOM.


## Problem 5 : OnClick Function Handling

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/5.q.png?raw=true)




## Problem 5 : Syntactical Error

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/5.bracket.png?raw=true)

- In the first one we call the function when the component renders hence it's not assigned to the onClick handler of the button as function pointer is not returned in the first case.

## Problem 5 : Fixed Code

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/5.ans.png?raw=true)

- In Second one, arrow function returns back the onClick handler function which is assigned to the onClick.






## Problem 6 : Syntactical Error

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/6.q.png?raw=true)
## Problem 6 : Syntactical Error

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/6.q.bool.png?raw=true)

- So Since, WrappedSingleListItem is expecting a boolean from isSelected variable. And this is the Most important variable as its solo work is to change the colour of the list items
## Problem 6 : Fixed Code 

![App Screenshot](https://github.com/Vivek17000/steeleyepics/blob/main/6.ans.png?raw=true)

- So for making it a working project at last we have to compare selectedindex with the map index as if both will be same then it means that item is selected.
## Screenshots Of Outputs

![](https://github.com/Vivek17000/steeleyepics/blob/main/op1.png?raw=true)
![](https://github.com/Vivek17000/steeleyepics/blob/main/op2.png?raw=true)
![](https://github.com/Vivek17000/steeleyepics/blob/main/op3.png?raw=true)
## Deployment

[netlify] - (https://steeleye-lpu-vivek.netlify.app/)

[github] - (https://github.com/Vivek17000/Vivek-Sharma_Front-End)



