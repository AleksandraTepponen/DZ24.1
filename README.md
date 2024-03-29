# Use Case Регистрация ЛК

<table>
<thead>
<tr>
<th id="Атрибуты/варианты использования/название поля" style="text-align:left;"> Атрибуты/варианты использования/название поля   </th>
<th id="Описание/ что содержит" style="text-align:left;"> Описание/ что содержит             </th>
</tr>
</thead>

<tbody>
<tr>
<td style="text-align:left;"><p>Краткое описание     </p></td>
<td style="text-align:left;"><p>Описывает процесс регистрации пользователя на сайте пиццерии / в ЛК      </p></td>
</tr>

<tr>
<td style="text-align:left;"><p>Действующее лицо    </p></td>
<td style="text-align:left;"><p>Неавторизованный пользователь / система   </p></td>
</tr>

<tr>
<td style="text-align:left;"><p>Предусловие  </p></td>
<td style="text-align:left;"><p>Неавторизованный пользователь находится на сайте пиццерии   </p></td>
</tr>

<tr>
<td style="text-align:left;"><p>Цель   </p></td>
<td style="text-align:left;"><p>Пользователь успешно зарегистрирован и направлено клиенту подтверждение об успешной регистрации   </p></td>
</tr>

</tbody>
</table>


## Основной сценарий

1. Пользователь переходит на страницу регистрации,
2. На экране авторизации есть выбор способа регистрации,
3. Пользователь выбирает способ регистрации с использованием электронной почты,
4. Пользователь вводит электронную почту,
5. Система проверяет актуальность введенных знаков (маска адреса электронной почты),
6. Пользователь нажимает кнопку **«ЗАРЕГИСТРИРОВАТЬСЯ»**,
7. На указанный адрес электронной почты система отправляет письмо о завершении регистрации и установлении пароля,
8. Пользователь переходит по ссылке из письма,
9. Пользователь вводит пароль,
10. Система проверяет актуальность введенных знаков (маска пароля),
11. Пользователь нажимает кнопку **«ПОДТВЕРДИТЬ»**,
12. На указанный адрес электронной почты система отправляет письмо о подтверждении регистрации.

## Альтернативный сценарий

1. *п.3.* Пользователь выбирает способ регистрации с использованием номера телефона, 
2. *п.4*. Пользователь вводит номер телефона, 
3. *п.5.* Система проверяет актуальность введенных знаков (маска адреса электронной почты), 
4. *п.7.* По указанному номер телефона система направляет сообщение о завершении регистрации и установлении пароля,
5. *п.8.* Пользователь переходит по ссылке из сообщения,
6. *п.12.* На указанный адрес номер телефона система отправляет сообщение о подтверждении регистрации.

## Исключение

* Если пользователь ввел некорректную информацию в строке электронной почты / номера телефона, и/или оставил незаполненными строки электронной почты / номера телефона – на экране будет выведено сообщение об ошибке «Некорректно указан логин».
* Если указанная электронная почта не соответствует указанной маске – система на экран выводит сообщение об ошибке «Некорректно указан логин».
