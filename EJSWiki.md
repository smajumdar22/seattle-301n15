Setting up EJS
Reference - https://www.youtube.com/watch?v=63IurQvsw9w


npm init -ynpm install --save express body-parser cors ejs
var bodyParser = require('body-parser')
var app = express();
app.use(bodyParser());app.use(cors());
app.set('views', path.join(__dirname,'views'));app.set('view engine','ejs');
app.listen(8000, function(request,response){response.render('index');});
app.listen(8000, function(){console.log("heard on 8000");});

Then create folder views > index.ejs

index.ejs ----  
<h1>Hello World</h1>
