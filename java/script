function addTask() {
  const name = document.getElementById("taskName").value;
  const days = document.getElementById("taskDays").value;
  const time = document.getElementById("taskTime").value;

  if (name === "" || days === "" || time === "") {
    alert("Please fill all fields");
    return;
  }

  const li = document.createElement("li");

  li.innerHTML = `
    <strong onclick="toggleTask(this)">${name}</strong><br>
    📅 Days: ${days}<br>
    ⏰ Schedule: ${new Date(time).toLocaleString()}
    <button class="delete-btn" onclick="deleteTask(this)">❌</button>
  `;

  document.getElementById("taskList").appendChild(li);

  // Clear inputs
  document.getElementById("taskName").value = "";
  document.getElementById("taskDays").value = "";
  document.getElementById("taskTime").value = "";
}

function deleteTask(btn) {
  btn.parentElement.remove();
}

function toggleTask(task) {
  task.parentElement.classList.toggle("completed");
}
