# XML
1. Создать внешний репозиторий c названием XML

3. Клонировать репозиторий XML на локальный компьютер

        $ git clone git@github.com:anyaignis/XML.git

3. Внутри локального XML создать файл “new.xml”

        $ touch "new.xml"

4. Добавить файл под гит

        $ git add "new.xml"

5. Закоммитить файл

        $ git commit -m "new file xml"

6. Отправить файл на внешний GitHub репозиторий

        $ git push

7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.

        vim new.xml
        <?xml version="1.0" encoding="UTF-8" ?>
        <about_me>
          <surname>Анна Жовтобрух</surname>
                <first_name>Анна</first_name>
                  <patronymic>Алексеевна</patronymic>
                          <age>28</age>
                <number_of_pets>1</number_of_pets>
          <desired_salary>500</desired_salary>
        </about_me>
        :wq

8. Отправить изменения на внешний репозиторий

        $ git add new.xml
        $ git commit -m "modified"
        $ git push

9. Создать файл preferences.xml

        $ touch preferences.xml

10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.

        $ vim preferences.xml
        <?xml version="1.0" encoding="UTF-8" ?>
        <preferences>
           <favorite_movie>Джентельмены</favorite_movie>
            <favorite_serial>Во все тяжкие</favorite_serial>
              <favorite_food>суши</favorite_food>
            <favorite_time_of_year>autumn</favorite_time_of_year>
           <country_to_visit>Norway</country_to_visit>
        </preferences>
        :wq

11. Создать файл skills.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML

        $ touch skills.xml
        $ vim skills.xml
        <?xml version="1.0" encoding="UTF-8" ?>
        <skills>
            <theory>
                <skill_1>testing_theory</skill_1>
                <skill_2>bug_reporting</skill_2>
                <skill_3>test_case</skill_3>
                <skill_4>check_list</skill_4>
                <skill_5>mobile_testing</skill_5>
            </theory>
            <web>
                <client_server_1>http_methods</client_server_1>
                <client_server_2>http_statuses</client_server_2>
                <client_server_3>json_xml_structures</client_server_3>
                <client_server_4>api_testing</client_server_4>
            </web>
            <tools>
                <tool_1>postman</tool_1>
                <tool_2>charles</tool_2>
                <tool_3>fiddler</tool_3>
                <tool_4>android_studio</tool_4>
                <tool_5>jmeter</tool_5>
                <tool_6>xcode</tool_6>
                <tool_7>dev_tools</tool_7>
            </tools>
            <row>
                <database>sql</database>
                <git_bash>commands</git_bash>
            </row>
        </skills>
        :wq

12. Сделать коммит в одну строку

        $ git commit preferences.xml skills.xml -m "new_files"

13. Отправить сразу 2 файла на внешний репозиторий

        $ git push -u

14. На веб интерфейсе создать файл bug_report.xml.
15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
18. Синхронизировать внешний и локальный репозиторий XML

        $ git pull

