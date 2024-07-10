Explanation: 
The above HTML code contains simple list tags and one text field which we will populate with text when we add, or delete tasks. Certain classes are assigned which we make use of while getting that particular element by DOM or by styling it inside the styles.css file. All the above content is inside a div with the class ‘container’ that has its own styling and attributes.

Explanation
Part 1: The way this function works is that it takes the ‘inputString’ i.e. the text that we pass inside the HTML text field as a task and then it creates several elements using DOM properties and appends their specific classes. After appending we insert all the elements inside the list as listItems.
Part 2: This addTask function is called when we click the button ‘addButton'(line 115) and then inside it we create a listItem with the value the user entered and then check the value, as it must not be an empty string then we simply add the above value inside the ‘inputTaskHolder’ and finally setting the value inside it as an empty string before calling the ‘bindFunction’.

Part 3: This code function is used to edit an existing task and we do so by keeping track of the parent node and then a simple if-else check whether the ‘editMode’ button is clicked or not if clicked then simply assign the value of the label innerText to value inside the editInput, if not then vice versa. Then after editing, we toggle the value of the ‘editMode’ as we have edited.

Part 4: In this part, we delete a task, and the way we do it is by making use of the parent node of the current node and then storing the parent of the parent node, and then simply deleting the child of this node.

Part 5: In this function, we mark the task as complete by simply appending the child of the parent node inside completeTaskHolder element and then calling the bindFunction.

Part 6:In this function, we mark the task as incomplete by simply appending the child of the parent node inside inCompleteTaskHolder element and then calling the bindFunction.

Part 7: In this part, we call the BindFunction where we respond to several user interaction activities and make several buttons work.

Part 8: In this final section, we iterate over several parts binding children with the help of for loop inside the incomplete and complete TaskHolder element.
