
todo_list = []
def add_task():
    task = input("Enter task to be added: ")
    todo_list.append(task)
    print("Task has been added \n")

def view_tasks():
    if not todo_list:
        print("No tasks available.\n")
        return

    print("\n TO DO LIST " )
    for i , task in enumerate(todo_list,start=1):
        print(f"{i}. {task}")
    print(" \n")

def delete_task():
    view_tasks()
    if not todo_list:
        return

    num = int(input("Ente task to be deleted: "))
    if 1 <=num <= len(todo_list):
        removed = todo_list.pop(num-1)
        print(f"Deleted task: {removed}\n")
    else:
              print("Invalid task number\n")


time_sessions = []

start_time = None
start_sessions = None 
current_subject = None 

def start_timer():
    global start_time , current_subject

    if start_time is not None:
        print("timer already running!")
        return

    current_subject= input("Enter the suject you want to study: ")
    start_time = time.time()
    print(f"Timer has been started for:{current_subject}\n")

def stop_timer():
    global start_time, current_subject

    if start_time is None:
        print("Timer is not running.\n")
        return

    end_time = time.time()
    duration = end_time - start_time

    minutes = duration/60

    session = {
        "subject": current_subject,
        "minutes": round(minutes, 2)
    }
    time_sessions.append(session)
    print(f"Timer stopped. You studied {current_subject} for [{round(minutes,2)} minutes.\n")

    start_time = None
    current_subject = None

def view_time_sessions():
    if not time_sessions:
        print("No timed sessions yet.\n")
        return

    print("\n Study time log")
    for i, s in enumerate(time_sessions,start=1):
        print(f"{i}.{s['subject']} - {s['minutes']}minutes")
        print("\n")

def main_menu():
    while True:
        print(" TO-DO LIST MENU ")
        print("1. ADD TASKS")
        print("2. VIEW TASKS")
        print("3. DELETE TASKS")
        print("4. START STUDY TIMER")
        print("5. STOP STUDY TIMER")
        print("6. VIEW TIMED SESSIONS")
        print("7. EXIT")

        choice= input ("enter your choice: ")
        if choice == "1":
            add_task()
        elif choice == "2":
            view_tasks()
        elif choice == "3":
            delete_task()
        elif choice == "4":
            start_timer()
        elif choice == "5":
            stop_timer()
        elif choice == "6":
            view_time_sessions()
        elif choice == "7":
            print("Exiting")
            break
        else:
            print("INVALID OPTION \n")

main_menu()

