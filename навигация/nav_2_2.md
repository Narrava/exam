# Разделы 2.2 - 2.5

## 2.2 Общие принципы и методы измерения параметров местоположения

Эффект Доплера

$$
    \Delta f(t) = -f_0 \cdot \dot{r}(t)/c \\
    f_1 = f_0 - f_0\frac{\dot{r}(t)}{c}
$$

## 2.3 Методы измерения разности времен

Если две точки расположены на расстоянии

$$
    \Delta r \equiv r_1 - r_2 = \lambda \\
    \Delta \varphi \equiv \varphi_1 - \varphi_2 = 2\pi
    \Delta r = \frac{\Delta\varphi\lambda}{2\pi}
$$

При этом на длину измерительной базы накладывается ограничение

$$
    d \equiv |O_1O_2| < \frac{\lambda}{2}
$$

Модуль разности фаз называют фазовым сдвигом. С развитием цифровых методов обработки сигналов широкое распространение получил способ, основанный на сравнении составляющих мгновенных фазовых спектров сигнала в этих точках. При этом фазовые спектры могут быть получены в результате Фурье-преобразования сигнала или других пр образований (например, Уолша, вейвлет, Вигнера и др.)

## 2.4 Частотный метод измерения разности дальностей

Измерение разности дальностей возможно на основе измерения доплеровского смещения частоты.

$$
    \Delta f_d = -f_0\frac{v_r}{c} = \frac{-v_r}{\lambda} = \frac{dr(t)}{dt}\frac{1}{\lambda}
$$

Если интегрировать Доплеровское смещение частоты

$$
    \intop_{t_k}^{t_{k+1}}\Delta f_d(t)dt = \frac{1}{\lambda}\intop_{t_k}^{t_{k+1}}\frac{dr(t)}{dt}dt = -\frac{1}{\lambda}|r_{k+1} - r_k| = -\frac{1}{\lambda}\Delta r_k
$$

Данный метод называют доплеровским интегральным. Он позволяет определить разности дальности от двух точек траекторий, в которых приемная станция находится в моменты времени $t_k$ и $t_{k+1p}$.

## 2.5 Методы измерения угловых величин

Амплитудный метод

Амплитудные методы пеленгования ИРИ основаны на том, что фазовые соотношения между сигналами, принимаемыми в пространственно разнесенных точках, можно преобразовать в амплитудную зависимость суммы принятых сигналов от местоположения ИРИ.

Наиболее очевидным и широко применяемым является амплитудный метод пеленгования, при котором используется антенная система, имеющая диаграмму направленности с ярко выраженным максимумом. В результате сканирования пространства определяется положение антенны, при котором выходной сигнал антенны имеет максимальную амплитуду, и направление, совпадающее с максимумом диаграммы направленности антенны, принимается за направление на ИРИ. Этот метод пеленгования можно рассматривать как вырожденный случай РДМ метода, когда за счет физического перемещения антенной системы подбирается такое ее положение, чтобы разности расстояний от ИРИ до симметричных точек отражателя зеркальной антенны были равны нулю (а, следовательно, и разности фаз сигналов, приходящих в эти точки были равны нулю). Синфазное сложение сигналов, пришедших по различным траекториям, обеспечивает максимум энергии в точке приема. При этом для каждой пары симметричных точек антенны, образующих измерительные базы, разность расстояний равна нулю и, следовательно, ПП ИРИ представляет собой плоскость, как вырожденный случай гиперболоида. Пересечение множества плоскостей, построенных относительно измерительных баз с общим центром, дает линию положения в виде прямой, проходящей через центр измерительных баз и перпендикулярной этим базам.

---

Фазовый метод

Фаза сигнала также содержит информацию об угловых координатах ИРИ. Поскольку множество точек пространства, фаза сигнала в которых постоянна, образует фронт электромагнитной волны, а нормаль к поверхности фронта совпадает с направлением распространения сигнала, то, посредством анализа фаз сигнала ИРИ в пространственно разнесенных точках, можно определить направление распространения электромагнитной волны, а, следовательно, и направление на ИРИ.

---

Временной метод

Принцип пеленгования на основе временного метода заключается в измерении разности времен приема сигналов от ИРИ двумя разнесенными антеннами. При отклонении положения ИРИ от перпендикуляра к центру базы возникает разность хода сигналов $\Delta r = r_1 − r_2$ . Относительное запаздывание $\tau$ сигналов, вследствие постоянства скорости и прямолинейности распространения радиоволн, пропорционально разности хода $\tau = \Delta r /c.$
Разность хода можно получить с помощью коррелятора. Есть разные схемы коррелятора (параллельная, с линией задержки, в пособии можно посмотреть).

---

Доплеровский метод (дифференциально доплеровский метод)

$$
    \Delta f_d = -\frac{v_r}{\lambda} \\
    \alpha = 2\arccos\left(\frac{v_r}{v}\right)
$$

Такой подход к измерению угла основан также на допущении о том, что при малых измерительных базах («малых» по сравнению с расстоянием до лоцируемого объекта) гиперболическая ПП асимптотически стремится к конической, которая в свою очередь однозначно описывается точкой вершины и углом при основании.
