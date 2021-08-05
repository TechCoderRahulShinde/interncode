# interncode
<script>

// Javascript program to find day of a given date

function solution(d, m, y)
{
	let t = [ 0, 3, 2, 5, 0, 3, 5, 1, 4, 6, 2, 4 ];
	y -= (m < 3) ? 1 : 0;
	return ( y + y/4 - y/100 + y/400 + t[m-1] + d) % 7;
}

// Driver Code

	let day = solution(30, 8, 2010);
	document.write(Math.round(day));

</script>
