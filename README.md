# ansible_role_ivcs_update
# Описание
Ansible роль для полностью автоматического обновления конфигурации серверов IVCS в кластере active-standvy, 2 головы и отдельно медиа сервера.
# Применение
Клонировать репозиторий

Изменить файл run-ivcs-update-example.yml - вставить ссылки на media и main ISO

Изменить файл hosts.yml - вписать IP адрес MAIN (HEAD) и MEDIA групп серверов, если используется аккаунт, отличный от admin - изменить.
# Запуск
ansible-playbook -i hosts.yml run-ivcs-update-example.yml -k -K

Указать пароль учетной записи с правами sudo и ssh для серверов
