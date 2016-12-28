# php-curl
a php curl function ,  get, post, post file and get cookie from cookie_file

Use:

$curl = new Curl();

 //for get 

$respone = $curl->get('http://test.com', array('key'=>'a'));
  
  
//for post 

$respone = $curl->post('http://test.com', array('key'=>'a'));
  
  
// post a file

  $respone = $curl->post('http://test.com', array('key'=>'a','file'=>'@'.'exist_file'), 1);
  
  
// how get the cookie from header

extractCookies(file_get_contents(_COOKIE_FILE));
