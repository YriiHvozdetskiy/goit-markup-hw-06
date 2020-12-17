# goit-markup-hw-06
1. нові svg іконки можна оптимізувати, зробити спрайт і вписати код іконки до старого спрайту
2. .form-item input:focus+label,.form-item input:not(:placeholder-shown)+label {
    transform: translate(-25px, -40px);
} --- не дозволяє таксту в label зїжати назад в input коли пропадає focus (якщо input заповнений) + це placeholder=" "
3. .form-item .checkbox {
    appearance: none;
    position: absolute;
    width: 1px;
    height: 1px;
    margin: -1px;
    border: 0;
    padding: 0;
    clip: rect(0 0 0 0);
    overflow: hidden;
} -- скриваєм стандартний чекбокс. задаєм рамку нашому чекбоксу.

.form-item .checkbox+.icon-check {
    fill: var(--bg-color-white);
} -- наш спрайт принімає колір чекбоксу

.form-item .checkbox:checked+.icon-check {
    background-color: var(--accent-color);
    border-color:var(--accent-color);
} -- коли стандартний чекбокс в стані чек наш кастомний чекбокс зміняю колір за макетом 