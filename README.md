# Добавление Microsoft Store в Windows 10 Enterprise LTSC  

Для Windows 10 Enterprise LTSC 2019   


## Для установки, запустите Add-Store.cmd от имени Администратора

Данный пакет добавляет только поддержку App Install и Purchase App. Xbox Identity вырезан и не будет установлен в любом случае.

Если Магазин не будет функционировать корректно, перезагрузитесь. Если всё ещё не работает, запустите Командную строку от имени Администратор, запустите следующие команды и перезагрузитесь повторно.

```PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage Microsoft.WindowsStore).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"```    

## Что ещё можно сделать при проблемах
>Щелчок правой кнопкой мыши по кнопке "Пуск"
>
>Выберите "Выполнить"
>
>Введите: WSReset.exe и нажмите "ОК"
>
>Будет выполнена очистка кэша Магазина

