<template>
    <div class="row">
        <div class="col-sm-12 col-md-6 col">
            <table class="table table-hover">
                <thead class="thead-default">
                    <tr>
                        <th>Size</th>
                        <th>Price</th>
                        <th>Add to basket</th>
                    </tr>
                    <tbody v-for="item in getMenuItems" >
                        <tr>
                            <td><strong> {{item.name}}</strong></td>
                    
                        <tr v-for="option in item.options">
                            <td> {{option.size }} </td>
                            <td> {{ option.price }}</td>
                            <td><button class="btn btn-sm btn-outline-success" type="button"> + </button></td>
                         </tr>
                    </tbody>
                </thead>
            </table>
        </div>
        <div class="col-sm-12 col-md-6 col">
       
        </div>
    </div>

</template>


<script>
    export default {
        data() {
            return {
                getMenuItems: {
                    1: {
                        'name': 'Margherita',
                        'description': 'A delicious tomato based pizza topped with mozzarella',
                        'options': [{
                            'size': 9,
                            'price': 6.95
                        }, {
                            'size': 12,
                            'price': 10.95
                        }]
                        },
                        2: {
                        'name': 'Pepperoni',
                        'description': 'A delicious tomato based pizza topped with mozzarella and pepperoni',
                        'options': [{
                            'size': 9,
                            'price': 7.95
                        }, {
                            'size': 12,
                            'price': 12.95
                        }]
                        },
                        3: {
                        'name': 'Ham and Pineapple',
                        'description': 'A delicious tomato based pizza topped with mozzarella, ham and pineapple',
                        'options': [{
                            'size': 9,
                            'price': 7.95
                        }, {
                            'size': 12,
                            'price': 12.95
                        }]
                        }

                }
            }
        }
    }
</script>