

## 1. Introdução

O Diagrama de Implantação é um dos diagramas estruturais da UML (Unified Modeling Language) e seu principal foco é descrever a arquitetura física de um sistema. Ele visualiza como os componentes de software (artefatos) são implantados em nós de hardware. Em essência, este diagrama oferece um mapa estático da topologia do hardware e a distribuição dos executáveis, bibliotecas e outros artefatos de software nesse hardware [1].

Ele é fundamental para entender o ambiente de execução, planejar a implantação, identificar gargalos de performance e facilitar a comunicação entre as equipes de desenvolvimento, operações e infraestrutura.

## 2. Objetivo

O principal objetivo deste documento é fornecer uma visão clara e unificada da arquitetura de implantação do sistema. Os objetivos específicos incluem:

* **Visualizar a Topologia do Hardware:** Apresentar os nós físicos (servidores, dispositivos) e a comunicação entre eles.
* **Mapear Software para Hardware:** Mostrar quais componentes de software (artefatos) são executados em quais nós de hardware.
* **Documentar a Configuração do Ambiente:** Servir como uma referência para a configuração e manutenção dos ambientes de desenvolvimento, teste e produção.
* **Apoiar o Planejamento de Escalabilidade e Manutenção:** Facilitar a análise de impacto de novas implantações e o planejamento de futuras expansões da infraestrutura.

## 3. Metodologia

Para a criação do diagrama, utilizamos a notação padrão da UML. Os principais elementos que compõem o diagrama de implantação são:

* **Nó (Node):** Representado como um cubo tridimensional, um nó é um recurso de hardware ou um ambiente de execução de software [1].
    * **Nó de Dispositivo (Device Node):** Representa um recurso computacional físico com capacidade de processamento, como um servidor de aplicação, servidor de banco de dados, ou um dispositivo móvel [1].
    * **Ambiente de Execução (Execution Environment Node):** Representa um ambiente de software específico que hospeda artefatos, como um sistema operacional, um container (Docker) ou um servidor de aplicação (Tomcat, JBoss) [1].

* **Artefato (Artifact):** Representa uma unidade física de software resultante do processo de desenvolvimento, como um arquivo `.jar`, `.war`, um executável, uma biblioteca (`.dll`) ou um script. É representado por um retângulo com o estereótipo `<<artifact>>` [1].

* **Associação de Comunicação (Communication Path):** Uma linha sólida que conecta dois nós, indicando que existe um caminho de comunicação entre eles. Frequentemente, o protocolo de comunicação (ex: `TCP/IP`, `HTTP/S`) é especificado na linha [1].

* **Dependência de Implantação (Deployment Relationship):** Uma linha tracejada com uma seta, geralmente com o estereótipo `<<deploy>>`, que conecta um nó a um artefato, indicando que o artefato é implantado naquele nó [1].

## 4. Diagramas de Implantação


<iframe width="768" height="432" src="https://miro.com/app/live-embed/uXjVJG7MFFY=/?embedMode=view_only_without_ui&moveToViewport=-724,-804,2137,1047&embedId=765887009438" frameborder="0" scrolling="no" allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen></iframe>

<p align="center">Autores: <a href="https://github.com/arthur-augusto">Arthur Augusto<a>, <a href="https://github.com/Gabrielfcoelho">Gabriel Flores<a>, <a href="https://github.com/igorvdaniel">Ígor Veras<a>, <a href="https://github.com/oyLeonardo">Leonardo Barcellos<a></a></p>

**Descrição:**
Este diagrama ilustra a arquitetura geral, incluindo os principais servidores, o banco de dados e a forma como os clientes interagem com o sistema.

---

## 5. Conclusão

O Diagrama de Implantação é uma ferramenta essencial para a documentação e planejamento da infraestrutura física e da distribuição de software. Ele proporciona uma base sólida para a tomada de decisões técnicas, otimização de recursos e garante que toda a equipe tenha uma compreensão comum de como o sistema funciona no mundo real, desde o hardware até os artefatos executáveis.

## 6. Referência Bibliográfica

1. UML deployment diagrams overview, common types of deployment diagrams - manifestation diagram, specification and instance level deployment diagram. Disponível em: <https://www.uml-diagrams.org/deployment-diagrams-overview.html>.

## 7. Histórico de Versão

| Versão | Data       | Autor         | Descrição  | Revisor | Data da Revisão |
|--------|------------|---------------|---------------------------------|------------|---------|
| 1.0    | 22/09/2025 | [Arthur Augusto](https://github.com/arthur-augusto), [Gabriel Flores](https://github.com/Gabrielfcoelho), [Ígor Veras](https://github.com/igorvdaniel), [Leonardo Barcelos](https://github.com/oyLeonardo)    | Criação da Documentação     |                                                    |