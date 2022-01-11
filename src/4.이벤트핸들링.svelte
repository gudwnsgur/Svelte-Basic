<script>
	
    // 	import {onMount} from 'svelte';
        
        let name = 'world';
        let isRed = false;
        
    // 	onMount(()=> {
    // 		const box = document.querySelector('.box');
    // 		box.addEventListener('click', ()=>{
    // 			isRed = !isRed;
    // 		})
    // 	})
        
        function enter() {
            name = 'enter';
        }
        function leave() {
            name = 'leave';
        }
        
    </script>
    
    <h1>Hello {name}!</h1>
    <div class = "box" 
             style = "background-color : {isRed ? 'red' : 'blue'};
                                color : white;"
             on:click={()=> {isRed = !isRed;}}
             on:mouseenter={enter}  
             on:mouseleave={()=>{leave()}}>
        <!-- on:event={func} : 기본적인 함수 사용법 -->
        <!-- on:event={ ()=> { func() } } : 함수에 매개변수가 필요할 때 이렇게 사용 -->
        Box!
    </div>
    
    
    
    <style>
        .box {
            width:300px;
            height:150px;
            background-color:orange;
        }
    </style>