#include <iostream>
#include <vector>
#include <fstream>
using namespace std;
struct employee {
    int id;
    string name;
    int salary;
};
employee inputEmpoyee() {
    cout<<"enter new employee data:"<<endl;
    employee emp;
    cout<<"enter id: ";
    cin>>emp.id;
    cout<<"enter name: ";
    cin>>emp.name;
    cout<<"enter salary: ";
    cin>>emp.salary;
    return emp;
}

void printEmployee(employee emp) {
    cout<<"id: "<<emp.id<<" "<<"name: "<<emp.name<<" "<<"salary: "<<emp.salary<<endl;
}
int main() {
    vector<employee> employees;
    employees.push_back(inputEmpoyee());
    employees.push_back(inputEmpoyee());

    for (employee e : employees ) {
        printEmployee(e);
    }

    ofstream storeEmployee("employee.txt", ios::app);
    for (employee e : employees) {
        storeEmployee<<e.id<<" "<<e.name<<" "<<e.salary<<endl;
    }
    return 0;
}
