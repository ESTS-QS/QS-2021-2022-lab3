# [Qualidade de Software 2020 2021](https://moodle.ips.pt/2122/course/view.php?id=311) - [ESTS IPS](https://www.estsetubal.ips.pt/)

## Laboratório 3

Este laboratório pretende a construção de uma bateria de testes sobre uma implementação de lista.

A estratégia de implementação deve ser uma lista simplesmente ligada.

Numa lista simplesmente ligada, os elementos são guardados dentro de nós que mantêm, além do elemento, um apontador para o próximo nó.

Os índices da lista começam em zero e vão até ao tamanho da lista menos um (`size()-1`).

# Tarefas

## Lista ligada

Considere a seguinte interface:

    interface List<E> {
        /**
        * Appends the element to the list.
        */
        void append(E element);

        /**
        * Returns the first element.
        */
        E first();

        /**
        * Returns the last element.
        */
        E last();

        /**
        * Returns the number of elements.
        */
        int size();

        /**
        * Returns the element at position `index`.
        * 
        * Positions start from zero.
        */
        E get(int index);

        /**~
        * Returns the position of the element.
        * 
        * If the element is not on the list, returns -1.
        */
        int find(E element);
    }

1. Implemente a interface como uma lista ligada
2. Construa um primeiro teste para o método `append()`
3. Defina uma *action* no GitHub de forma a executar os testes sempre que ocorre um `commit`
4. Conclua a bateria de testes, assegurando cobertura de 100%
