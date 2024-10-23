#Sri
class Task:
    def __init__(self, title, description, assigned_to, deadline):
        self.title = title
        self.description = description
        self.assigned_to = assigned_to
        self.deadline = deadline
        self.completed = False

    def mark_complete(self):
        self.completed = True

    def __str__(self):
        status = "Completed" if self.completed else "In Progress"
        return f"Task: {self.title} | Status: {status} | Assigned to: {self.assigned_to} | Deadline: {self.deadline}"

# Example usage:
task1 = Task("Design UI", "Create a new interface for Project Nexus", "Alice", "2024-11-01")
print(task1)
task1.mark_complete()
print(task1)
