<script lang="ts">
  import Counter from './lib/Counter.svelte'
  import * as THREE from 'three';

// init

const camera = new THREE.PerspectiveCamera( 70, window.innerWidth / window.innerHeight, 0.01, 10 );
camera.position.z = 1;

const scene = new THREE.Scene();

const geometry = new THREE.BoxGeometry( 0.2, 0.2, 0.2 );
const material = new THREE.MeshNormalMaterial();

const mesh = new THREE.Mesh( geometry, material );
scene.add( mesh );

const renderer = new THREE.WebGLRenderer( { antialias: true } );
renderer.setSize( window.innerWidth, window.innerHeight );
renderer.setAnimationLoop( animation );
document.body.appendChild( renderer.domElement );

// animation

function animation( time ) {

	mesh.rotation.x = time / 2000;
	mesh.rotation.y = time / 1000;

	renderer.render( scene, camera );

}
  
</script>
<main>

  <h1>Portfolio Site 0.0.1</h1>

  <div class="card">
    <Counter />
  </div>

  <p>
    Check out <a href="https://github.com/willettAMT" target="_blank" rel="noreferrer">my github</a>, friends!
  </p>

</main>

<style>

</style>
