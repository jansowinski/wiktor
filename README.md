## Wymagania

Działa tylko na mac os sierra. Wymaga [imagesnap](http://iharder.sourceforge.net/current/macosx/imagesnap/) i [sterowników](https://github.com/adrianmihalko/ch340g-ch34g-ch34x-mac-os-x-driver) do aruino nano.

- [Arduino IDE](https://www.arduino.cc/en/Guide/ArduinoNano)
- [PIR](https://forbot.pl/blog/kurs-arduino-ii-4-przerwania-kontaktron-czujnik-pir-id16792)
- [Instrukcja działania czujnika PIR](https://www.youtube.com/watch?v=63TR_3kn76U)

## Co jest czym

`main.go` - po odpaleniu / skompilowaniu czyta z serialportu i w momencie gdy dostanie stringa "BANG!" odpala zdjęcie z kamerki w komputerze (`snap()`) oraz wysyła keystroke do odpowieniej aplikacji (do rozbudowania w `sendCommand()`).