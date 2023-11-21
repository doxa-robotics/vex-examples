category: sensing  
signature: RemoteControlCodeEnabled = true;  
description: Enables or disables Controller configured actions from the Devices menu.

# Controller Enable/Disable

```cpp
RemoteControlCodeEnabled = false;
```

Увімкнення або вимкнення налаштованих дій контролера з меню пристроїв. 

## Як це працює

Встановіть увімкнення або вимкнення налаштованих дій контролера, надавши команді RemoteControlCodeEnabled значення `true` або `false`. За замовчуванням, контролер увімкнено в кожному проєкті.

## Приклад

Налаштовані дії у цьому прикладі використовуються для керуванням трансмісією і встановлюються у налаштуваннях контролера в меню пристроїв.

![configured_action](configured_action.png)

У цьому прикладі налаштовані дії контролера вимкнені на початку роботи програми.

Потім, робот проїде вперед 150 мм.

Зрештою, команда **RemoteControlCodeEnabled** вмикає контролер для відновлення керування роботом із контролера.

```cpp
RemoteControlCodeEnabled = false;
Drivetrain.driveFor(forward, 150, mm);
RemoteControlCodeEnabled = true;
```

<advanced>
</advanced>