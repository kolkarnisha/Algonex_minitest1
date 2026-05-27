# Algonex_minitest1

def get_grade(marks):
 

    if marks >= 90:
        print( "A+")
    elif marks >= 80:
        print("A")
    elif marks >= 70:
        print("B")
    elif marks >= 60:
        print("C")
    elif marks >= 50:
        print( "D")
    else:
        print( "F")

test_marks = [95, 82, 71, 55, 45]

for marks in test_marks:
    grade = get_grade(marks)
    print(f"{marks} {grade}")

#2.answer
def check_eligibility(cgpa, has_backlogs, github_projects, branch):
    
    
   
    rule1 = cgpa >= 7.0 and not has_backlogs
    
    rule2 = cgpa >= 6.5 and github_projects >= 3
    
    
    eligible = rule1 or rule2
    
   
    priority = ["CSE", "IT"]
    
   
    if eligible:
        if priority:
            print( "Eligible with Priority")
        else:
            print( "Eligible")
    else:
        print( "Not Eligible")


students = [
    {"name": "Nisha", "cgpa": 8.2, "backlogs": False, "githubprojects": 1, "branch": "CSE"},
    {"name": "taj", "cgpa": 6.8, "backlogs": False, "githubprojects": 4, "branch": "IT"},   
    {"name": "zareen", "cgpa": 7.5, "backlogs": True, "githubprojects": 5, "branch":'b.com'}]
print(students)
