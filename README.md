# QA-Postman

Создать запросы в Postman.

Protocol: http
IP: 162.55.220.72
Port: 5005

EP_1
Method: GET
EndPoint: /get_method
request url params: 
 name: str
 age: int

response: 
[
    “Str”,
    “Str”
]


[
  "Greck", 
  "31"
]

==================

EP_2
Method: POST
EndPoint: /user_info_3
request form data: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}}



{
    "age": "31",
    "family": {
        "children": [
            [
                "Alex",
                24
            ],
            [
                "Kate",
                12
            ]
        ],
        "u_salary_1_5_year": 3800
    },
    "name": "Greck",
    "salary": 950
}
==================

EP_3
Method: GET
EndPoint: /object_info_1
request url params: 
 name: str
 age: int
 weight: int

response: 
{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}



{
    "age": 31,
    "daily_food": 1.02,
    "daily_sleep": 212.5,
    "name": "Greck"
}
==================

EP_4
Method: GET
EndPoint: /object_info_2
request url params: 
 name: str
 age: int
 salary: int

response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }


{
    "person": {
        "u_age": 31,
        "u_name": [
            "Greck",
            950,
            31
        ],
        "u_salary_5_years": 3990.0
    },
    "qa_salary_after_1.5_year": 3135.0,
    "qa_salary_after_12_months": 2565.0,
    "qa_salary_after_3.5_years": 3610.0,
    "qa_salary_after_6_months": 1900,
    "start_qa_salary": 950
}

==================

EP_5
Method: GET
EndPoint: /object_info_3
request url params: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }



{
    "age": "31",
    "family": {
        "children": [
            [
                "Alex",
                24
            ],
            [
                "Kate",
                12
            ]
        ],
        "pets": {
            "cat": {
                "age": 3,
                "name": "Sunny"
            },
            "dog": {
                "age": 4,
                "name": "Luky"
            }
        },
        "u_salary_1_5_year": 3800
    },
    "name": "Greck",
    "salary": 950
}
==================

EP_6
Method: GET
EndPoint: /object_info_4
request url params: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2), str(salary * 3)]}


{
    "age": 31,
    "name": "Greck",
    "salary": [
        950,
        "1900",
        "2850"
    ]
}

==================

EP_7
Method: POST
EndPoint: /user_info_2
request form data: 
 name: str
 age: int
 salary: int

response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }

{
    "person": {
        "u_age": 31,
        "u_name": [
            "Greck",
            950,
            31
        ],
        "u_salary_5_years": 3990.0
    },
    "qa_salary_after_1.5_year": 3135.0,
    "qa_salary_after_12_months": 2565.0,
    "qa_salary_after_3.5_years": 3610.0,
    "qa_salary_after_6_months": 1900,
    "start_qa_salary": 950
}
