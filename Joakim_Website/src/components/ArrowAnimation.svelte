
<div class="arrow">
</div>

<style>
div.arrow {
	width: 3vmin;
	height: 3vmin;
	box-sizing: border-box;
	left: 50%;
	top: 50%;
	transform: rotate(45deg);
	
	&::before {
		content: '';
		width: 100%;
		height: 100%;
		border-width: .8vmin .8vmin 0 0;
		border-style: solid;
		border-color: #fafafa;
		transition: .2s ease;
		display: block;
		transform-origin: 100% 0;
	}

	
	&:after {
		content: '';
		float: left;
		position: relative;
		top: -100%;
		width: 100%;
		height: 100%;
		border-width: 0 .6vmin 0 0;
		border-style: solid;
		border-color: #fafafa;
		transform-origin: 100% 0;
		transition:.2s ease;
	}
	
	&:hover::after {
		transform: rotate(45deg);
		border-color: gray;
		height: 110%;
	}
	&:hover::before {
		border-color: gray;
		transform: scale(.8);
		
	}
	
}
</style>