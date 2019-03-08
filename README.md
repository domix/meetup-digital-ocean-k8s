# meetup-digital-ocean-k8s

Primero aprovisionar el cluster de k8s en la consola de DO

Una vez aprovisionado, descargar el `kubeconfig` file.

Configurar `kubectl` para que use el `kubeconfig`descargado.

Se procede a instalar el contenedor de pruebas

    $ kubectl apply -f deployment.yaml

Se configura el `LoadBalancer`

    $ kubectl apply -f service-load-balancer.yaml

Podemos obtener la ip con:

    $ kubectl get services