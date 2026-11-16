# Работа по теме «Работа с серверами и протокол удалённого управления SSH»

Работу выполнил Квасной Роман Борисович

## 1. Установка SSH-клиента и генерация ключевой пары
- Проверка клиента SSH: “ssh -V” → OpenSSH_10.2p1.
<img width="245" height="64" alt="{155183CB-9B81-4636-A6C7-0ED218E77532}" src="https://github.com/user-attachments/assets/f96a46ca-2ac9-421a-983e-8869e1fff2c7" /><img width="160" height="32" alt="{1F0BD23F-A98D-44DA-BF3F-0D042C11F8E3}" src="https://github.com/user-attachments/assets/adcaf89f-5058-4bf5-a811-42156bc37e16" />
- Проверка наличия и версии git: “git --version” → git version 2.53.0.
![Uploading {1F0BD23F-A98D-44DA-BF3F-0D042C11F8E3}.png…]()
- Сгенерирована пара ключей ed25519 с паролем:
  ‘ssh-keygen -t ed25519 -C “romankvasnoy@gmail.com”’

- Проверка ключей: “ls -la ~/.ssh”

- Отпечаток публичного ключа: “ssh-keygen -l -f ~/.ssh/id_ed25519.pub”

- Настройка ssh-agent для ввода без пароля:
