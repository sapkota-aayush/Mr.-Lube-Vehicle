<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Mr. Lube Vehicle Management Software</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
      max-width: 800px;
    }
    h1, h2, h3, h4 {
      color: #333;
    }
    pre {
      background-color: #f4f4f4;
      padding: 10px;
      overflow: auto;
    }
    code {
      background-color: #f4f4f4;
      padding: 2px 4px;
    }
    a {
      color: #0066cc;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    hr {
      border: 0;
      height: 1px;
      background: #ccc;
      margin: 20px 0;
    }
    ul, ol {
      margin-left: 20px;
    }
  </style>
</head>
<body>
  <h1>Mr. Lube Vehicle Management Software</h1>
  
  <h2>Overview</h2>
  <p>
    This project is an imitation of the <strong>Mr. Lube Automotive Repairing Software</strong>, inspired by my past work as a technician at Mr. Lube. The software is built using <strong>C++ and MySQL</strong>, with a strong emphasis on <strong>Object-Oriented Programming (OOP)</strong> principles.
  </p>
  
  <h2>Key Features</h2>
  <ul>
    <li>✅ Add vehicle information and check if it exists in the database.</li>
    <li>✅ Retrieve previous service history.</li>
    <li>✅ Perform new services and update the database.</li>
    <li>✅ Process payments and view payment history.</li>
    <li>✅ Send receipts to customers via email using the <strong>SendGrid API</strong>.</li>
    <li>✅ Secure authentication system for users.</li>
    <li>✅ Uses <strong>cURL</strong> for HTTP requests and <strong>nlohmann/json</strong> for JSON handling.</li>
    <li>✅ Graphical User Interface (GUI) built with <strong>Qt</strong> for an enhanced user experience.</li>
  </ul>
  
  <hr>
  
  <h2>Project Structure</h2>
  <p>
    The project consists of <strong>11 files</strong>: <strong>5 header files</strong> and their corresponding <strong>5 implementation files</strong>, along with <code>main.cpp</code> as the entry point.
  </p>
  
  <h3>Header Files (.h)</h3>
  <ul>
    <li><code>authsystem.h</code> - Handles authentication.</li>
    <li><code>services.h</code> - Manages vehicle services.</li>
    <li><code>payment.h</code> - Handles payment transactions.</li>
    <li><code>utility.h</code> - Contains utility functions (e.g., validation).</li>
    <li><code>vehicle.h</code> - Manages vehicle data and service history.</li>
  </ul>
  
  <h3>Source Files (.cpp)</h3>
  <ul>
    <li><code>authsystem.cpp</code> - Implements authentication logic.</li>
    <li><code>services.cpp</code> - Implements service functionalities.</li>
    <li><code>payment.cpp</code> - Implements payment processing.</li>
    <li><code>utility.cpp</code> - Implements utility/helper functions.</li>
    <li><code>vehicle.cpp</code> - Implements vehicle management.</li>
    <li><code>main.cpp</code> - The main entry point that ties everything together.</li>
  </ul>
  
  <hr>
  
  <h2>Installation Guide</h2>
  <ol>
    <li>
      <h3>Install MySQL and Configure Database</h3>
      <p>
        Follow this guide to set up MySQL in <strong>Visual Studio</strong> for a C++ application:
        <a href="https://www.geeksforgeeks.org/how-to-setup-mysql-database-in-visual-studio-2022-for-a-cpp-application/" target="_blank">MySQL Setup Guide</a>
      </p>
    </li>
    <li>
      <h3>Install Required Libraries</h3>
      <h4>nlohmann/json (for JSON parsing)</h4>
      <p>
        Install the <strong>nlohmann/json</strong> library via vcpkg:
      </p>
      <pre><code>vcpkg install nlohmann-json</code></pre>
      <p>
        Or download it manually from the <a href="https://github.com/nlohmann/json" target="_blank">nlohmann/json GitHub repository</a>.
      </p>
      
      <h4>cURL (for HTTP requests - Sending emails via API)</h4>
      <ol>
        <li>
          Install cURL on Windows:
          <pre><code>vcpkg install curl</code></pre>
        </li>
        <li>
          Link cURL to your C++ project in <strong>Visual Studio</strong>:
          <ul>
            <li>Go to <code>Project Properties &gt; C/C++ &gt; Additional Include Directories</code></li>
            <li>Add the path to cURL's include directory.</li>
          </ul>
        </li>
      </ol>
      
      <h4>Qt (for GUI development)</h4>
      <ol>
        <li>
          Download and install <strong>Qt</strong> from the <a href="https://www.qt.io/download" target="_blank">Qt Official Site</a>.
        </li>
        <li>
          Configure Qt in your development environment:
          <ul>
            <li>Add Qt include and library paths to your project settings.</li>
            <li>Ensure the correct Qt version is selected in your IDE.</li>
          </ul>
        </li>
      </ol>
    </li>
  </ol>
  
  <hr>
  
  <h2>Usage</h2>
  <ol>
    <li><strong>Authentication</strong> - Log in to the system.</li>
    <li><strong>Vehicle Lookup</strong> - Enter vehicle details to check service history.</li>
    <li><strong>Service Addition</strong> - Add new services to the selected vehicle.</li>
    <li><strong>Payment Processing</strong> - Handle payments and generate receipts.</li>
    <li><strong>Email Receipt</strong> - Send a receipt to the customer via the <strong>SendGrid API</strong>.</li>
    <li><strong>User Interface</strong> - Perform all operations using the <strong>Qt-based GUI</strong>.</li>
  </ol>
  
  <h3>API Configuration (SendGrid for Email)</h3>
  <ol>
    <li>
      Sign up at <a href="https://sendgrid.com/" target="_blank">SendGrid</a>.
    </li>
    <li>
      Generate an <strong>API key</strong>.
    </li>
    <li>
      Store the key in an environment variable or a config file.
    </li>
  </ol>
  
  <hr>
  
  <h2>Screenshots / Demonstrations</h2>
  <p>
    Due to some Visual Studio Code 2022 issues, I have not pushed the code yet. However, you can view the screenshots and demonstrations of the software via this 
    <a href="https://drive.google.com/drive/folders/1ZiZqaWQw60EVPBj5M2eHIkZEjItIH7yC" target="_blank">Google Drive folder</a>.
  </p>
  
  <hr>
  
  <h2>Why This Project?</h2>
  <p>
    This project is a practical demonstration of how <strong>OOP (Object-Oriented Programming)</strong> simplifies software design and maintenance by abstracting underlying complexity. It mimics real-world software used in the automotive industry to manage vehicle services efficiently.
  </p>
  
  <hr>
  
  <h2>Future Enhancements</h2>
  <ul>
    <li>Expand GUI features with more interactive elements.</li>
    <li>Implement multi-user authentication roles (e.g., Admin, Technician).</li>
    <li>Improve error handling and logging.</li>
    <li>Expand email templates for better customer communication.</li>
  </ul>
  
  <hr>
  
  <h2>Reference Project</h2>
  <p>
    For additional inspiration, check out this <strong>Insurance Management</strong> system: 
    <a href="https://github.com/sumitkumar1503/insurancemanagement/blob/master/README.md" target="_blank">Insurance Management on GitHub</a>.
  </p>
  
  <hr>
  
  <h2>Contributor</h2>
  <p>👨‍💻 <strong>Aayush Sapkota</strong></p>
  <p>💡 <em>Feel free to contribute, suggest improvements, or fork this repository!</em> 🚀</p>
</body>
</html>
