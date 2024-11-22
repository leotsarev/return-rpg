+++
title="Солдат"
+++

{% mermaid() %}
graph TD
    caban[<b>Кабан спускается с холма 5</b><br>После того персонаж атакует в ближнем бою после маневра, которым подошел к оппоненту, он может потратить <span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span><span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span><span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span> или <span title="Triumph symbol" class="genesys-symbol genesys-symbol-triumph"></span> чтобы сшибить врага с ног и заставить его отойти на одну дистанцию]
    caban --> caban2[<b>Кабан спускается с горы 10</b><br>После того как персонаж подошел к оппоненту маневром, он может потратить 2 усталости и добавить <span title="Success symbol" class="genesys-symbol genesys-symbol-success"></span><span title="Success symbol" class="genesys-symbol genesys-symbol-success"></span><span title="Threat symbol" class="genesys-symbol genesys-symbol-threat"></span><span title="Threat symbol" class="genesys-symbol genesys-symbol-threat"></span> к проверке ближнего боя в этом ходу]


    def["<b>Защитная стойка 5</b> <br/>Один раз за раунд, потрать Х усталости (не больше, чем  ранг Защитной Стойки). До конца следующего хода сложность попадания по тебе в ближнем бою выше на Х"]
    hit2[<b>Закаленный 10</b><br/>Порог ран +2]
    hit4[<b>Закаленный 20</b><br/>Порог ран +2]
    parry[<b>Парирование 5</b><br/>Когда получает ущерб от атаки в ближнем бою, но держит при этом оружие или щит, можето потратить 3 усталости, чтобы снизить ущерб на 2+ранг -- перед Поглощением]

        cmd[<b>Командное звание 5</b> <br/>Имеет законные права командовать солдатами; получает <span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span> при бросках лидерства в этом случае, а солдаты <span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span> при бросках Выдержки.]
    

    resilience[<b>Героическая стойкость 15 </b><br/>Потрать 1 очко сюжета: снизь ущерб на ранг своей Стойкости]

    block[<b>Блок 10</b> <br />Если держит щит, может использовать Парирование против выстрелов.]
    bulwark[<b>Прикрыть друга 10</b> <br />Если держит щит, может использовать Парирование, когда бьют союзника, находящегося вплотную.]

    bodyguard["<b>Телохранитель 15</b> <br />Один раз раунд, потрать Х усталости (не больше ранга телохранителя), выбери Х слюзников, находящихся вплотную, чтобы повысить сложность атак против них на Х до конца твоего следующего хода."]
    bodyguard2["<b>Телохранитель 25</b> <br />Один раз раунд, потрать Х усталости (не больше ранга телохранителя), выбери Х слюзников, находящихся вплотную, чтобы повысить сложность атак против них на Х до конца твоего следующего хода."]
    
    back2back[<b>Спина к спине 20</b> <br />Пока вплотную хотя с одним союзником, ты и союзник добавляют <span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span> к боевым броскам. Если у союзника тоже есть этот таланат, то кумулятивно до <span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span><span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span>.]

    attrup["<b>Повышение 25</b><br>Любая характеристика увеличивается на 1 (максимум 6)"]
    
    block --> armormaster[<b>Мастер доспехов 15</b> <br/>+1 Поглощение, пока надет доспех]
    armormaster --> armormaster2[<b>Тяжелые доспехи 20</b> <br/>Если доспех приносит 2 или больше поглощения, он приносит и +1/+1 защиту]
    def3["<b>Защитная стойка 15</b> <br/>Один раз за раунд, потрать Х усталости (не больше, чем  ранг Защитной Стойки). До конца следующего хода сложность попадания по тебе в ближнем бою выше на Х"]
    defensive[<b>Оборона 20</b><br /> +1/+1 к защите]
    prehit["<b>Предотвратить 25</b><br>Один раз за раунд, когда враг в досягаемости атакует союзника, потрать 1 очко сюжета, чтобы немедленно автоматически попасть по нему атакой. Попадание снимает ущерб оружия + возможные бонусы и случается перед броском атаки врага"]

    indomitable["<b>Неуязвимый 25</b><br>Один раз за сцену, когда персонаж должен потерять сознание от избытка ран или усталости: потрать 1 очко сюжета, он не теряет сознание до конца своего следующего хода и не может потерять его никаким образом."]

    hit2 --> resilience --> hit4

    def  -->  hit2 

    parry --> bulwark & block

    bulwark --> bodyguard 

    hit2 -->  def3 --> defensive

    bodyguard & def3 --> back2back --> bodyguard2 & prehit

    hit4 --> attrup

    armormaster2 --> indomitable


    classDef active stroke-width:15px, stroke: 	#8B0000
{% end %}