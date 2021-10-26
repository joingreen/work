<script context="module">
	export const prerender = true;
</script>

<script>


	let a=[
		{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},{
			type:"KH 72",
			model:"86274vc010",
			rev:12,
			oldrev:11,
			drawAt:1633870927800,
			doneAt:1633870927800,
		},
	]

function dateString(timeNum){
	let time=new Date(timeNum)
	console.log(time.getDate())
	return `${time.getDate()}/${time.getMonth()+1}`
}
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>
<div class="input-group mb-3" style="max-width:500px;position:sticky " >
		<input type="text" class="form-control" placeholder="Search">
		<div class="input-group-append">
		  <span class="input-group-text">12</span>
		  
		</div>
	  </div>
<section>
	<table class="table">
		<thead>
		  <tr class="table-success">
			<th scope="col">#</th>
			<th scope="col">Model</th>
			<th scope="col">Rev</th>
			<th scope="col">Drawing</th>
			<th scope="col">Done</th>
		  </tr>
		</thead>
		<tbody>
			{#each a as todo, i}
			<tr>
				<td scope="row" class="text-secondary">{i}</td>
				<th>{todo.model}</th>
				<td>{todo.rev}_{todo.oldrev}</td>
				<td><small>{dateString(todo.drawAt)}</small></td>
				<td><small>{dateString(todo.doneAt)}</small></td>
			  </tr>
			{/each}
		 
		</tbody>
	  </table>
</section>


<style>
	*{letter-spacing: -1px;}
</style>