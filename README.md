# JSON2XML-php-converter

#HowToUse
    $response = your json code;
    
    $responsex= json_encode($response);
    // Require Array2XML class which takes a PHP array and changes it to XML
    require_once('array2xml.php');
    // Gets JSON file
    // Decodes JSON into a PHP array
    $php_array = json_decode($result, true);
    // adding Content Type
    
    // Converts PHP Array to XML with the root element being 'root-element-here'
    $xml = Array2XML::createXML('myroot', $php_array);
    $result=$xml->saveXML();
    
    
    echo $result;
