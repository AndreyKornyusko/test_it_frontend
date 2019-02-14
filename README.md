# Проект TEST_IT

================short rules for working with this repository for developers================
1) Клонируете себе на машину репозиторий: 
1.1) git clone https://github.com/VitaliiKalinbet/test_it_frontend.git
2) Закрываете консоль и открываете ее в созданной после клонирования папке (или cd test_it_frontend). Создаете ветку с названием компонента который будете делать, например: 
2.1) git checkout -b Home
2.2) Чтобы установить все модули, на уровне с package.json запускаете консоль и команда:
npm i
2.3) Ознакомьтесь с установленными модулями в package.json, и старайтесь ими обойтись, например для графиков это react-chartjs-2, для прогресс бара react-sweet-progress.
3) Работаете в ветке например (Home), первая отправка файлов на репозиторий: 
3.1) git add .
3.2) git commit -m "some text"
3.3) git push --set-upstream origin Home       (при повторных отправках на этом шаге просто - git push) 


=================INFORMATION FOR DEVELOPERS===================
В компонент App.jsx подключены 4 страницы согласно макета home.psd это HomePage.jsx, page-1.psd это InstructionPage.jsx, page-2(3).psd это TestPage.jsx, result.psd это ResultPage.jsx. Подключен роутинг, в зависимости от окончания url, страницы переключаются, переходы между страницами реализуйте у себя с помощью <NavLink to='/…'>.
Макеты тут: 
https://drive.google.com/drive/folders/1KQrr1w8U9VyH-qVJqQ5icF_ywVw81Nnb

Frontend разработчиков в команде 6, соответственно мы сделали 6 компонентов ‘src/components’:
1) Header 
2) Home 
3) Instruction
4) ProgressBar
5) Result
6) Test (создает Михаил Малков) 
Еще у нас 5 фронтендщиков и 5 компонентов, пожалуйста разбирайте кто чем занимается и пишите тут, буду помечать. 

Какую работу мы ожидаем от Вас с каждым компонентом: 
1) Клонируете себе репозиторий, создаете ветку по названию своего компонента, и дальше только в ней работаете (в ветку "master" НИКОГДА НИЧЕГО НЕ ПУШИМ, только в свою. Короткие правила работы с GitHub опишу в README.md репозитория)
2) Создаете разметку прямо в своем реакт - компоненте. И ее стилизируете в одноименном файле с окончанием '.module.css' он лежит всегда рядом и уже импортирован в Ваш компонент. 
CSS модули, как с ними работать: 
https://www.youtube.com/watch?v=bQ3UPYFHyJ0
  2.1) Размещаете блоки  flex'ами
  2.2) По принципу mobile first, наслаиваете css правила
  2.3) Шрифты от дизайнера в папке 'assets/fonts'
  2.4) Картинки, кому потребуются, складывать  'assets/img'
  2.5) Цвета напишем тут позже, использовать именно их в css
3) Потом в свою созданную ветку (НЕ В master !!!) отправляете промежуточные результаты работы, чтобы все их видели
