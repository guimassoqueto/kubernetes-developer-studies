## Definiçãokubectl get pods


Um pod pode ter vários contêineres executando aplicativos dentro dele, mas também pode ter um ou mais contêineres de inicialização, que são executados antes de os contêineres de aplicativos serem iniciados.

Os contêineres de inicialização são exatamente como os contêineres normais, exceto:

Os contêineres de inicialização sempre são executados até a conclusão.
Cada contêiner init deve ser concluído com êxito antes que o próximo seja iniciado.

Se o contêiner de inicialização de um pod falhar, o kubelet reiniciará repetidamente esse contêiner de inicialização até que seja bem-sucedido. No entanto, se o Pod tiver um restartPolicy de Never e um contêiner init falhar durante a inicialização desse Pod, o Kubernetes tratará o Pod geral como com falha.