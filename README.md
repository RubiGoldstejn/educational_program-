# educational_program-
# Инициализация словаря с образовательной программой
educational_program = {
    "math": ["algebra", "geometry", "trigonometry"],
    "science": ["biology", "chemistry", "physics"],
    "history": ["ancient history", "world history", "modern history"]
}

# Функция для вывода содержания образовательной программы
def print_educational_program(program):
    print("Educational Program:")
    for subject, topics in program.items():
        print(f"{subject}:")
        for topic in topics:
            print(f"- {topic}")

# Функция для добавления новой темы к определенному предмету
def add_topic(program, subject, topic):
    if subject in program:
        program[subject].append(topic)
    else:
        print("Invalid subject")

# Вывод содержания образовательной программы
print_educational_program(educational_program)

# Добавление новой темы к математике
add_topic(educational_program, "math", "calculus")

# Вывод обновленного содержания образовательной программы
print_educational_program(educational_program)
