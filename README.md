is_running = True
collections = ["task1, task2"]

def show_collection(task_collection):
    print("======")
    for i, j in enumerate(task_collection):
        print(i + 1, j)
    print("======")

    def show_menu():
        print("1 - посмотреть задачу \n"
              "2 - добавить задач \n"
              "3 - редактировать \n"
              "4 - удалить \n"
              "5- выход")

print("добро пожаловать")

while is_running:
    show_menu()
    choice_user = input("введите свой выбор")
    match str(choice_user):
        case '1':
            show_collection(collections)
        case '2':
            add_task = input("введите имя")
            collections.append(add_task)
        case '3':
            show_collection(collections)
            select_task = int(input("введите номер задачи"))
            edit_task = input("введите новое имя задачи для редактирования")
            collections[select_task -1] = edit_task
        case '4':
            show_collection(collections)
            delete_task = int(input("введите новое имя задачи для удаления"))
            collections.pop(delete_task -1)
        case '5':
            is_running = False
            print("до свидания")
        case _:
            print("такого пункта нет")
# 1semestr
