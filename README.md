if __name__ == '__main__':
    # Input the number of students
    n = int(input("Enter the number of students: "))

    # Create a nested list to store student names and grades
    students = []
    for _ in range(n):
        name = input("Enter the student name: ")
        grade = float(input("Enter the student grade: "))
        students.append([name, grade])

    # Find the second lowest grade
    unique_grades = sorted(set(student[1] for student in students))
    second_lowest_grade = unique_grades[1]

    # Find students with the second lowest grade
    second_lowest_students = [student[0] for student in students if student[1] == second_lowest_grade]

    # Sort the names alphabetically
    second_lowest_students.sort()

    # Print the names of students with the second lowest grade
    print("\nStudents with the second lowest grade:")
    for student in second_lowest_students:
        print(student)
# Homework Aydın S.
