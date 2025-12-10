O NLB opera na **Camada 4** (TCP/UDP) e suas verificações de integridade são basicamente de conectividade de rede, **não detectando falhas no nível da aplicação HTTP**.

Para aceitar o tráfego UDP, você precisa de um **Network Load Balancer (NLB)** ou instâncias EC2 como endpoint, pois o ALB só suporta HTTP/HTTPS.