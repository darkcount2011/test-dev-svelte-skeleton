<script>
</script>

<div class="grid grid-cols-3 h-16 w-full">
	<div class="">
		<slot name="lead">(lead)</slot>
	</div>
	<div>
		<slot />
	</div>
	<div class="">
		<slot name="trail">(trail)</slot>
	</div>
</div>
