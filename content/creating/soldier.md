+++
title="Таланты: Солдат"
weight=101
+++

{% mermaid() %}
graph TD
    

    caban[<b>Кабан спускается с холма 5</b><br>После того персонаж атакует в ближнем бою после маневра, которым подошел к оппоненту, он может потратить <span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span><span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span><span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span> или <span title="Triumph symbol" class="genesys-symbol genesys-symbol-triumph"></span> чтобы сшибить врага с ног и заставить его отойти на одну дистанцию]
    caban --> caban2[<b>Кабан спускается с горы 10</b><br>После того как персонаж подошел к оппоненту маневром, он может потратить 2 усталости и добавить <span title="Success symbol" class="genesys-symbol genesys-symbol-success"></span><span title="Success symbol" class="genesys-symbol genesys-symbol-success"></span><span title="Threat symbol" class="genesys-symbol genesys-symbol-threat"></span><span title="Threat symbol" class="genesys-symbol genesys-symbol-threat"></span> к проверке ближнего боя в этом ходу]


    def["<b>Привычка к львиноголову 5</b> <br/>Львиноголов восстанавливает на 1 рану больше за каждый ранг привычки."]
    hit2[<b>Закаленный 10</b><br/>Порог ран +2]
    hit4[<b>Закаленный 20</b><br/>Порог ран +2]
    parry[<b>Парирование 5</b><br/>Когда получает ущерб от атаки в ближнем бою, но держит при этом оружие или щит, можете потратить 3 усталости, чтобы снизить ущерб на 2+ранг -- перед Поглощением]

    cmd[<b>Командное звание 5</b> <br/>Имеет законные права командовать солдатами; получает <span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span> при бросках лидерства в этом случае, а солдаты <span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span> при бросках Выдержки.]
    

    resilience[<b>Героическая стойкость 15 </b><br/>Потрать 1 очко сюжета: снизь нанесенный ущерб на ранг своей Стойкости]

    block[<b>Блок 15</b> <br />Если держит щит, может использовать Парирование против выстрелов. Считается рангом Парирования.]
    bulwark[<b>Прикрыть друга 10</b> <br />Если держит щит, может использовать Парирование, когда бьют союзника, находящегося вплотную. Считается рангом Парирования.]

    bodyguard["<b>Телохранитель 15</b> <br />Один раз раунд, потрать Х усталости (не больше ранга телохранителя), выбери Х союзников, находящихся вплотную, чтобы повысить сложность атак против них на Х до конца твоего следующего хода."]
    bodyguard2["<b>Телохранитель 25</b> <br />Один раз раунд, потрать Х усталости (не больше ранга телохранителя), выбери Х союзников, находящихся вплотную, чтобы повысить сложность атак против них на Х до конца твоего следующего хода."]
    
    back2back[<b>Спина к спине 20</b> <br />Пока вплотную хотя с одним союзником, ты и союзник добавляют <span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span> к боевым броскам. Если у союзника тоже есть этот талант, то кумулятивно до <span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span><span title="Boost dice" class="genesys-symbol genesys-symbol-boost"></span>.]

    attrup["<b>Повышение 25</b><br>Любая характеристика увеличивается на 1 (максимум 6)"]
    
    block --> armormaster[<b>Мастер доспехов 20</b> <br/>+1 Поглощение, пока надет доспех]
    armormaster --> armormaster2[<b>Тяжелые доспехи 25</b> <br/>Если доспех приносит 3+ поглощения, он приносит и +1/+1 защиту]
     defensive[<b>Оборона 20</b><br /> +1/+1 к защите]
    def3["<b>Привычка к львиноголову 15</b> <br/>Львиноголов восстанавливает на 1 рану больше за каждый ранг привычки."]
    prehit["<b>Предотвратить 25</b><br>Один раз за сцену, когда враг в досягаемости атакует союзника, потрать 1 очко сюжета, чтобы немедленно автоматически попасть по нему атакой. Попадание снимает ущерб оружия + возможные бонусы и случается перед броском атаки врага"]


    cmd --> coord_attack[<b>Командный голос 10</b><br>1 раз за раунд, как маневр: союзники на ближней дистанции в количестве, равном рангу Лидерства, получают <span title="Advantage symbol" class="genesys-symbol genesys-symbol-advantage"></span> при атаках до начала следующего хода.]
    hit2 --> resilience --> hit4

    def  -->  hit2 

    parry --> bulwark
    
    bulwark --> bodyguard 
    bulwark --> block

    hit2 -->  def3 --> defensive

    bodyguard --> back2back --> bodyguard2 & prehit

    hit4 --> attrup

    classDef active stroke-width:15px, stroke: 	#8B0000
{% end %}