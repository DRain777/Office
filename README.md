Установка Office
Создаем отдльную папку,можно назвать office,в нее устанавливаем office,удаляем первые 3 файла оставляем только office 2021.
в этой же папки через shift и правой кнопки мыши открываем Power_shall, и вводим команды
first_command:
reg add "HKCU\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\Ecs" /v "CountryCode" /t REG_SZ /d "std::wstring|US" /f
next_command:
.\setup.exe /configure .\configuration-Office2021Enterprise.xml
