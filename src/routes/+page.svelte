<script>
	import { data } from '../stores/data.js';
	import foto from '$lib/images/fotoRaulIsai.png';
	import flecha from '$lib/images/down.png';
    import planets from '$lib/images/planets.png';
    import pistadown from '$lib/images/pista-down.png';
</script>

<div class="intro" id="intro">
	<div class="left">
		<div class="imgContainer">
			<img class="imgDev" src={planets} alt="foto de developer" />
		</div>
	</div>
	<div class="right">
		<div class="wrapper">
			<h2>Hi There, Im</h2>
			<h1>{data.NameResum}</h1>
			<h3>Freelancer <span /></h3>
		</div>
		<a href="#portafolio">
			<img class="imgFlecha" src={pistadown} alt="flecha abajo" />
		</a>
	</div>
</div>


<style>
.intro {
    display: flex;
}
.left {
    flex: 0.5;
    overflow: hidden;
}
.imgContainer {
      width: 700px;
      height: 700px;
      background-color: rgb(0, 0, 0);
      border-radius: 50%;
      display: flex;
      align-items: flex-end;
      justify-content: center;
      float: right;
    }
    .imgDev {
        height: 100%;   
    }
    .right {
        flex: 0.5;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    } 
    .wrapper {
      width: 100%;
      height: 100%;
      padding-left: 50px;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
    h1 {
        font-size: 60px;
        margin: 10px 0; 
        color: aliceblue;
        margin-right: 30%;
    }
    h2 {
        font-size: 30px;
        margin: 10px 0;
    }
    h3 {
        font-size: 20px;
        margin: 10px 0;
    }
    span {
        font-size: inherit;
          color: crimson;
    }

    .imgFlecha {
        width: 40%;
        animation: arrowBlink 2s infinite;
      }

    
</style>
