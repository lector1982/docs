### Включення масиву чи об'єкта до набору плейсхолдерів

*Примітка: використовує метод toPlaceholder.*

void toPlaceholders(mixed $subject[, string $prefix]);

**$subject** - масив чи об'єкт зі значеннями.
**$prefix** - префікс, що буде доданий перед назвою плейсхолдера.
За замовчуванням: порожньо.

***

#### Приклад.

	// Задамо деякий масив, який може видати наш сніпет:
	
	$a = array( 'name' => 'Спільнота MODX', 
				'type' => 'site', 
				'url' => 'http://modx.im' 
			  ); 
	// Додамо в набір плейсхолдерів:
	$modx->toPlaceholders($a,'test.'); 
	
	// Виведемо текст для перевірки плейсхолдерів:
	echo ' Назва сайту: [+test.name+]<br> Посилання на сайт: [+test.url+] '; 
	
	// Отримаємо результат: 
	// Назва сайту: Спільнота MODX 
	// Посилання на сайт: http://modx.im
