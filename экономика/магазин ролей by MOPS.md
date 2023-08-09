{% set money = member.getAttribute('money') %}
{% if  arguments == null %}
{% elseif arguments == 'алмаз' %}
{% require money.value >= 15000 returning 'У вас недостаточно алмазов для покупки данной роли!' %}
{% do money.decrement(15000) %}
{% do member.addRole(айди роли) %}
Вы успешно купили роль <@&1068896014016200816> - Теперь вы самый блатной на этом сервере:emoji_21: <:emoji_36:968532555982864395> 
{% elseif arguments == 'изумруд' %}
{% require money.value >= 30000 returning 'У вас недостаточно алмазов для покупки данной роли!' %}
{% do money.decrement(30000) %}
{% do member.addRole(айди роли) %}
Вы успешно купили роль <@&1068896916689137804> - Теперь вы самый редкий на этом сервере <:emoji_36:968532555982864395> 
{% elseif arguments == 'незерит' %}
{% require money.value >= 50000 returning 'У вас недостаточно алмазов для покупки данной роли!' %}
{% do money.decrement(50000) %}
{% do member.addRole(айди роли) %}
Вы успешно купили роль <@&1068896137177739274> - Теперь вы самый трудный на этом сервере <:emoji_36:968532555982864395> 
{% elseif arguments == 'порох' %}
{% require money.value >= 100000 returning 'У вас недостаточно алмазов для покупки данной роли!' %}
{% do money.decrement(100000) %}
{% do member.addRole(айди роли) %}
Вы успешно купили роль <@&1080214017471172668> - Теперь вы самый взрывной на этом сервере <:emoji_36:968532555982864395> 
{% endif %}