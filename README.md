# JSON2XML-php-converter

#HowToUse

    $json = your json code;
    // Require Array2XML class which takes a PHP array and changes it to XML
    require_once('array2xml.php');
    // Gets JSON file
    // Decodes JSON into a PHP array
    $php_array = json_decode($json, true);
    // adding Content Type
    
    // Converts PHP Array to XML with the root element being 'root-element-here'
    $xml = Array2XML::createXML('myroot', $php_array);
    $result=$xml->saveXML();
    
    
    echo $result;
