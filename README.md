1. add btn

// Add update button functionality
	var uBtn = document.createElement("button");
	uBtn.appendChild(document.createTextNode("Update"));
	li.appendChild(uBtn);
	uBtn.addEventListener("click", updateListItem);
}

//
enterButton.addEventListener("click",addListAfterClick);
input.addEventListener("keypress", addListAfterKeypress);

//
function updateListItem(event) {
	var updatedText = prompt("Enter the updated text:");
	var li = event.target.parentElement; // Get the parent li element
	li.textContent = updatedText; // Update the text content of the li element
}
