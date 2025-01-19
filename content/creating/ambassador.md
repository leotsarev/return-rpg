+++
title="Таланты: Посланник"
weight=112
draft=true
+++

Посланник
===

{% mermaid() %}
graph TD


    уверенная_речь ~~~  вдохновляющая_речь & чтение_эмоций ~~~ Благоприятный ~~~ письменные_подтверждения & делай_как_я

    уверенная_речь[<b>Уверенная речь 5</b> <br> Если про броске социального навыка выкинул <span title="Триумф" class="genesys-symbol genesys-symbol-triumph"></span>, добавь <span title="adv" class="genesys-symbol genesys-symbol-success"></span>]

        делай_как_я[<b>Делай как я 20 </b> <br> После успеха в броске, потрать 1 усталость: Х персонажей, где Х — твой ранг в лидерстве, получат автоматический <span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span> в одной проверке этого же навыка до конца следующего хода.]

            письменные_подтверждения[<b>Письменные подтверждения 20 </b> <br> Помогая персонажу с Обаянием, Обманом, Лидерством или Переговорами, добавь автоматический <span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span> в дополнение к общим правилам.]


    вдохновляющая_речь[<b>Вдохновляющая речь 10</b><br>Проверь Лидерство против <span title="Сложность" class="genesys-symbol genesys-symbol-difficulty"></span><span title="Сложность" class="genesys-symbol genesys-symbol-difficulty"></span>. За каждый <span title="adv" class="genesys-symbol genesys-symbol-success"></span> или <span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span> один союзник на короткой дистанции восстанавливает 1 усталость.]

    чтение_эмоций[<b>Чтение эмоций 10</b><br> Добавь <span title="Голубой" class="genesys-symbol genesys-symbol-boost"></span> ко всем проверкам Обмана, Запугивания или Обаяния.]

    Благоприятный[<b>Благоприятный 15</b><br>Потрать 1 усталость, чтобы снизить сложность броска Обаяния или Переговоров]

    classDef active stroke-width:15px, stroke: 	#8B0000
{% end %}
