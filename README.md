# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #4 выполнил(а):
- Лещишин Роман Александрович
- РИ-210914

Отметка о выполнении заданий (заполняется студентом):
| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | # | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## 4. Лабораторная работа. "Перцептрон"
## Цель работы
Обучение перцептрона производить вычисления OR, AND, NAND, XOR в проекте Unity.

## Задание 1
В проекте Unity реализовать перцептрон, который умеет производить вычисления OR, AND, NAND, XOR
Сцена в Unity:
![image](https://user-images.githubusercontent.com/114608473/207903921-99f68ff8-da40-47f9-8521-5dee59599300.png)
Вычисление OR
На 1 эпохе, перцептрон не успел обучиться, значит слишко мало.
![Image_1ORtr1](https://user-images.githubusercontent.com/114608473/207904208-fc7c7521-ca2e-4b74-ac64-eb246914aa6e.jpg)
На 3 эпохе значение ошибки осталось тем же.
![Image_1ORtr3](https://user-images.githubusercontent.com/114608473/207904593-91e3f7f4-a760-405d-851e-5d7a3c85b728.jpg)
Перцептрон обучился на 5 эпохе.
![Image_1ORtr5](https://user-images.githubusercontent.com/114608473/207904728-ac2ce7c9-1599-4753-9b4f-18daa57412c2.jpg)
Для закрепления проверил значение ошибки на 8 эпохах.
![Image_1ORtr8](https://user-images.githubusercontent.com/114608473/207904889-4fec54c5-ba1e-4a67-b0a4-78c9856e9e56.jpg)
Вычисление AND
Для обучения этой операции перцептрону потребовалось больше эпох, чем в OR.
![Image_2ANDtr1](https://user-images.githubusercontent.com/114608473/207905229-f851b8c2-949b-4249-93c0-dea48901d101.jpg)
![Image_2ANDtr9](https://user-images.githubusercontent.com/114608473/207905283-a98c19b1-adaa-43c3-a14f-20977c0f1ed0.jpg)
Из значений ошибки можно придти к выводу, что перцептрону для успешного обучения нужно как минимум 9 эпох.
Вычисление NAND
Значения ошибки при обучении очень похожи на операцию AND.
![Image_3NANDtr1](https://user-images.githubusercontent.com/114608473/207906562-ede778b6-1dbe-430e-b210-f6fd606caf08.jpg)
![Image_3NANDtr8](https://user-images.githubusercontent.com/114608473/207906588-0e6b0f58-32df-4212-8021-4b2cf0cb7a95.jpg)
Вычисление XOR
При увеличении количества эпох, значение ошибки только увеличивается, что доказывает утверждение Minsky о XOR problem.
![Image_4XORtr1](https://user-images.githubusercontent.com/114608473/207906987-701830bf-15a5-40f2-a9da-45b73587267b.jpg)
![Image_4XORtr16](https://user-images.githubusercontent.com/114608473/207907081-9f2c0f6b-f1da-4884-a0bc-2dfdf3f077f0.jpg)
Перцепторон может обучаться вычислению только линейных функций, а XOR таковой не является.
## Задание 2
Комментарии к файлу rollerball_config:
![ImageRollerBallConfig](https://user-images.githubusercontent.com/114608473/206841484-71d4f133-b81b-450c-8f5b-32e708ced661.jpg)
Вывод: игровой баланс заключается в достижении определенного уровня фана, при котором игра не кажется слишком сложной, но в то же время в неё интересно играть и пользователь получает удовольствие от игры. Использование систем машинного обучения позволяет проводить большое количество тестов с различными параметрами, выявлять элементы игры, которые нарушают баланс, изменять эти элементы и снова проводить тесты, добиваясь равновесия в игре. Благодаря таким системам разработчики тратят меньше времени на тестировании различных стратегий и лучше выявляют элементы дисбаланса.
## Задание 3
### Какова роль параметра Lr? Ответьте на вопрос, приведите пример выполнения кода, который подтверждает ваш ответ. В качестве эксперимента можете изменить значение параметра.

- Перечисленные в этом туториале действия могут быть выполнены запуском на исполнение скрипт-файла, доступного [в репозитории](https://github.com/Den1sovDm1triy/hfss-scripting/blob/main/ScreatingSphereInAEDT.py).
- Для запуска скрипт-файла откройте Ansys Electronics Desktop. Перейдите во вкладку [Automation] - [Run Script] - [Выберите файл с именем ScreatingSphereInAEDT.py из репозитория].

```py

import ScriptEnv
ScriptEnv.Initialize("Ansoft.ElectronicsDesktop")
oDesktop.RestoreWindow()
oProject = oDesktop.NewProject()
oProject.Rename("C:/Users/denisov.dv/Documents/Ansoft/SphereDIffraction.aedt", True)
oProject.InsertDesign("HFSS", "HFSSDesign1", "HFSS Terminal Network", "")
oDesign = oProject.SetActiveDesign("HFSSDesign1")
oEditor = oDesign.SetActiveEditor("3D Modeler")
oEditor.CreateSphere(
	[
		"NAME:SphereParameters",
		"XCenter:="		, "0mm",
		"YCenter:="		, "0mm",
		"ZCenter:="		, "0mm",
		"Radius:="		, "1.0770329614269mm"
	], 
)

```

## Выводы

Абзац умных слов о том, что было сделано и что было узнано.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
