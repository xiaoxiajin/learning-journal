# Dec 10, 2024

## React Hook

```javascript
const [isOpenModal, setisOpenModal] = useState(false);

return(
<Button className="countryDrop" onClick={()=>{setisOpenModal(true)}}>
 </Button>

<Dialog open={isOpenModal} onClose={()=>setisOpenModal(false)} className="locationModal">
// onClose handle close when click outside
    <Button className="close_ " onClick={()=>{setisOpenModal(false)}}><IoIosClose/></Button>
</Dialog>
)
```

# Dec 9, 2024

## install bootstrap

1. add `"bootstrap": "^4.1.3"` in package.json "dependencies": {}
2. `npm install`
3. `import "bootstrap/dist/css/bootstrap.min.css"` in App.js

## some useful websites for install

1. https://mui.com/material-ui/getting-started/installation/
2. https://www.npmjs.com/package/bootstrap-4-react
3. https://www.npmjs.com/package/react-icons
