height:   `0px` |  `auto`

transitionDuration: number

transitionTimingFunction: 'linear' ....

```javascript

let foldTimer;

function Demo(){
	const [isFold, setIsFold] = useState(true);
	return (
		<>
			<AutoHeight
				transitionDuration={2000}
				transitionFunc={'ease'}
				height={isFold ? '0px', 'auto'}
				ref={autoHeightDivRef}
			>
				{children}
			</AutoHeight>
		</>
	)
}

```