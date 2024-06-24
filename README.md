# PINN
Практическое задание по курсу Нейросетевые методы численного решения дифференциальных уравнений

PINN - physically informed neural network - архитектура нейросети, с помощью которой в данном задании решается начально-краевая задача для уравнения в частных производных (формулировку см. в файле pde_formulation.jpeg).
Для решения использовалась библиотека deepxde, само решение см. в файле mypinn.ipynb. По ходу обучения нейросети происходило обучение коэффициента lambda. Обучение проводилось для 3-х начальных приближений lambda: 0, 10 и 20.
Во всех случаях процесс обучения стабилизировался при значении lambda=16. Для каждого начального приближения обучение проходило в несколько этапов, причём для каждого следующего этапа происходило понижение learning rate.
