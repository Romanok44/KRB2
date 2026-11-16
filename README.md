# Работа по теме «Работа с серверами и протокол удалённого управления SSH»

Работу выполнил Квасной Роман Борисович

## 1. Установка SSH-клиента и генерация ключевой пары
- Проверка клиента SSH: “ssh -V” → OpenSSH_10.2p1.

  <img width="245" height="64" alt="1" src="https://github.com/user-attachments/assets/61d0cace-36ce-4bca-8963-47ad77d2dd0d" />

- Проверка наличия и версии git: “git --version” → git version 2.53.0.

  <img width="160" height="32" alt="2" src="https://github.com/user-attachments/assets/c821be54-3d2f-4a40-88cc-e5aeeda3ba51" />

- Сгенерирована пара ключей ed25519 с паролем:
  ‘ssh-keygen -t ed25519 -C “romankvasnoy@gmail.com”’

- Проверка ключей: “ls -la ~/.ssh”

- Отпечаток публичного ключа: “ssh-keygen -l -f ~/.ssh/id_ed25519.pub”

- Настройка ssh-agent для ввода без пароля:
