<template>
    <h1 class="title">Order List</h1>
    <section class="new-order">
        <table class="table">
            <thead>
                <tr>
                    <td> ID</td>
                    <td><i class='bx bxs-user' ></i> Name</td>
                    <td><i class='bx bx-detail'></i> Description</td>
                    <td><i class='bx bx-money'></i> Price</td>
                </tr>
            </thead>
            <tbody>
                <tr :key="order.id" v-for="order in order_list">
                    <td>{{order.id}}</td>
                    <td>{{order.name}}</td>
                    <td>{{order.description}}</td>
                    <td>${{order.price}}</td>
                </tr>
            </tbody>
        </table>
    </section>
</template>

<script>
export default {
    setup() {

        const order_list = [
            {
                id: 1,
                name:   'Tenis',
                description: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry',
                price: 10.00
            },
            {
                id: 2,
                name:   'Convite pro show de happy hour',
                description: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry',
                price: 25.00
            },
            {
                id: 3,
                name:   'Computador da Xuxa',
                description: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry',
                price: 50.00
            },
            {
                id: 4,
                name:   'Computador da lucas',
                description: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry',
                price: 100.00
            },
        ]

        return { order_list }
    }
}
</script>

<style lang="scss">
    
    .title {
        margin-left: 30px;
        margin-top: 30px;
        font-weight: normal;
    }
    
    .new-order {
        margin-top: 30px;
        margin-left: 30px;
        margin-right: 30px;
        border-top: 4px solid var(--primary);
        background-color: var(--white);

        p {
            font-size: 2rem;
        }
    }

    .table {
        width: 100%;
        overflow-x: auto;        
        thead {
            background-color:var(--gray-light);
        }

        tr:hover td {
            background: var(--primary);
        }

        td {
            padding: 10px;
            transition: all 0.8s ease-out;

            &:nth-of-type(4) {
                width: 150px;
            }
        }
    }  

</style>