<template>

    <div>
        <Card :key="monster.id" monster="monster"></Card>
    </div>

</template>

<script>

import Card from '../card/Card.component'

export default {
    props:{
        
    }
}


// export const CardList = props => {
//     return <div className="card-list">
//         {props.monsters.map(monster => (
//             <Card key={monster.id} monster={monster}/>
//           ))}
//     </div>
// }
</script>