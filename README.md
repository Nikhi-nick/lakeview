Lake View Resturant
DEPLOYING A STATIC WEBSITE INTO AZURE USING AZURE SERVICES
PROJECT DETAILS:
   1. PROJECT DEMO TUTORIAL: Demo link 
    2. PROJECT WEBSITE URL: Website link
ROLES AND RESPONSIBILITIES:
1.	M. Nikhil (Website deployment and recording the demo.)
2.	G. Bhavani (Managing the Documentation and code deployment)
3.	N. Ramsai (Data Collection)


PROBLEM STATEMENT

Context: A restaurant is looking to establish a strong online presence by creating a static website that showcases its menu, location, hours of operation, and other essential information. The website needs to be fast, reliable, and scalable, capable of handling a growing customer base. The restaurant management seeks to deploy this website on a cloud platform with minimal infrastructure management and low operational costs.
Challenge: The restaurant’s team lacks the in-house expertise to manage complex servers or infrastructure and is seeking a cloud solution that simplifies the process of hosting and maintaining a static website. Additionally, the website needs to be accessible globally, load quickly, and remain highly available with the ability to automatically scale during peak times (e.g., promotional events, holidays).
PROJECT DESCRIPTION

This project involves deploying a static restaurant website using Microsoft Azure cloud services. The website will showcase the restaurant’s menu, location, and contact information. Azure Blob Storage will host the static files, while Azure CDN ensures fast, global content delivery. Azure DNS will manage custom domain names. The solution is scalable, cost-effective, and requires minimal maintenance, providing the restaurant with a reliable, high-performance online presence

AZURE SERVICES USED

1.	Azure storage account 
2.	Azure static website 
3.	Azure containers
4.	Azure data protection
5.	Azure backup vault
6.	Azure AI services: QnA makers, language service, chatbot.

AZURE STORAGE ACCOUNT:

An Azure Storage Account is a cloud-based service provided by Microsoft Azure that allows users to store and manage various types of data in a secure and scalable manner. It supports different storage services, including Blob Storage for unstructured data (like images and videos), File Storage for file shares, Queue Storage for messaging, and Table Storage for NoSQL data. 

With an Azure Storage Account, users can easily access their data from anywhere, integrate with other Azure services, and benefit from features like redundancy, backup, and security options. It is designed to handle large amounts of data efficiently, making it ideal for applications ranging from simple websites to complex enterprise solutions.

AZURE STATIC WEBSITE:

Azure Static Website is a feature of Azure Storage that enables users to host static web applications directly from a storage account. It allows developers to serve HTML, CSS, JavaScript, and other static files without the need for a backend server. This service is ideal for hosting personal blogs, portfolios, documentation, or any site that doesn't require dynamic content generation.

With Azure Static Website, users benefit from high availability, scalability, and global distribution through Azure's Content Delivery Network (CDN). It also supports custom domain names and provides secure access via HTTPS. The setup is straightforward, making it easy to deploy and manage static sites efficiently while taking advantage of Azure's robust infrastructure.

AZURE CONTAINERS:

Azure Containers are a service offered by Microsoft Azure that allows users to deploy and manage containerized applications in the cloud. Containers are lightweight, portable units that package an application and its dependencies, ensuring consistent performance across different environments. Azure provides several options for working with containers, including Azure Kubernetes Service (AKS) for orchestrating and managing container clusters, and Azure Container Instances (ACI) for running containers without the need for complex orchestration.

Using Azure Containers, developers can easily scale applications, improve resource utilization, and enhance deployment speed. This service supports various container images and integrates seamlessly with other Azure services, making it ideal for modern cloud-native applications and microservices architectures.

AZURE DATA PROTECTION:

Azure Data Protection Service is a solution from Microsoft Azure designed to safeguard data across various environments. It includes features like Azure Backup for secure data backup, Azure Site Recovery for disaster recovery, advanced security measures to protect against threats, and tools to ensure compliance with regulations. Overall, it helps organizations keep their data safe, recoverable, and compliant.

AZURE BACKUP VAULT:

Azure Backup Vault is a storage solution in Microsoft Azure that securely stores backup data. It allows centralized management of backups for Azure resources and on-premises servers. Key features include built-in security with data encryption, customizable retention policies for compliance, and cost management options. Overall, it helps ensure your backup data is organized and protected.

AZURE AI SERVICES:

Azure AI services provide a comprehensive suite of tools and APIs that enable developers to build intelligent applications. These services include Azure Machine Learning for creating and deploying machine learning models, Cognitive Services for integrating features like image and speech recognition, Azure Bot Services for developing chatbots, and Azure Cognitive Search for enhancing search capabilities with AI. Together, they empower businesses to leverage artificial intelligence to improve user experiences and streamline operations.

SOURCE CODE

<!DOCTYPE html>
<html lang="en">

<head>

     <title>Lake View restaurant</title>
     <!-- 

Eatery Cafe Template 

http://www.templatemo.com/tm-515-eatery

-->
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=Edge">
     <meta name="description" content="">
     <meta name="keywords" content="">
     <meta name="author" content="">
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

     <link rel="stylesheet" href="css/bootstrap.min.css">
     <link rel="stylesheet" href="css/font-awesome.min.css">
     <link rel="stylesheet" href="css/animate.css">
     <link rel="stylesheet" href="css/owl.carousel.css">
     <link rel="stylesheet" href="css/owl.theme.default.min.css">
     <link rel="stylesheet" href="css/magnific-popup.css">

     <!-- MAIN CSS -->
     <link rel="stylesheet" href="css/templatemo-style.css">

</head>

<body>

     <!-- PRE LOADER -->
     <section class="preloader">
          <div class="spinner">

               <span class="spinner-rotate"></span>

          </div>
     </section>

     <!-- MENU -->
     <section class="navbar custom-navbar navbar-fixed-top" role="navigation">
          <div class="container">

               <div class="navbar-header">
                    <button class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
                         <span class="icon icon-bar"></span>
                         <span class="icon icon-bar"></span>
                         <span class="icon icon-bar"></span>
                    </button>

                    <!-- lOGO TEXT HERE -->
                    <a href="index.html" class="navbar-brand">Lake <span>.</span> View :)</a>
               </div>

               <!-- MENU LINKS -->
               <div class="collapse navbar-collapse">
                    <ul class="nav navbar-nav navbar-nav-first">
                         <li><a href="#home" class="smoothScroll">Home</a></li>
                         <li><a href="#about" class="smoothScroll">About</a></li>
                         <!-- <li><a href="#team" class="smoothScroll">Chef</a></li> -->
                         <li><a href="#menu" class="smoothScroll">Menu</a></li>
                         <!-- <li><a href="#contact" class="smoothScroll">Contact</a></li> -->
                         <li><a href="chatbot.html" class="smoothScroll">Chatbot</a></li>
                    </ul>

                    <ul class="nav navbar-nav navbar-right">
                         <li><a href="#">Call Now! <i class="fa fa-phone"></i>+91 9876543210</a></li>
                         <a href="#footer" class="section-btn">Reserve a table</a>
                    </ul>
               </div>

          </div>
     </section>

     <!-- HOME -->
     <section id="home" class="slider" data-stellar-background-ratio="0.5">
          <div class="row">

               <div class="owl-carousel owl-theme">
                    <div class="item item-first">
                         <div class="caption">
                              <div class="container">
                                   <div class="col-md-8 col-sm-12">
                                        <h1>Lake View :) Restaurant</h1>
                                        <h1>Our mission is to provide an unforgettable experience</h1>
                                        <a href="#team" class="section-btn btn btn-default smoothScroll">Meet our
                                             chef</a>
                                   </div>
                              </div>
                         </div>
                    </div>

                    <div class="item item-second">
                         <div class="caption">
                              <div class="container">
                                   <div class="col-md-8 col-sm-12">
                                        <h3>Your Perfect Breakfast</h3>
                                        <h1>The best dinning quality can be here too!</h1>
                                        <a href="#menu" class="section-btn btn btn-default smoothScroll">Discover
                                             menu</a>
                                   </div>
                              </div>
                         </div>
                    </div>

                    <div class="item item-third">
                         <div class="caption">
                              <div class="container">
                                   <div class="col-md-8 col-sm-12">
                                        <h3>New Restaurant in Town</h3>
                                        <h1>Enjoy our special menus every Sunday and Friday</h1>
                                        <a href="#contact"
                                             class="section-btn btn btn-default smoothScroll">Reservation</a>
                                   </div>
                              </div>
                         </div>
                    </div>
               </div>

          </div>
     </section>

     <!-- ABOUT -->
     <section id="about" data-stellar-background-ratio="0.5">
          <div class="container">
               <div class="row">

                    <div class="col-md-6 col-sm-12">
                         <div class="about-info">
                              <div class="section-title wow fadeInUp" data-wow-delay="0.2s">
                                   <h4>Read our story</h4>
                                   <h2>We've been Making The Delicious Foods Since 1999</h2>
                              </div>

                              <div class="wow fadeInUp" data-wow-delay="0.4s">
                                   <p> Since we first opened our doors, our passion for creating delicious food has been
                                        at the heart of everything we do. Established in 1999, LAKE VIEW has grown from
                                        a simple idea into a beloved destination for food lovers in Hyderbad.

                                        At our core, we believe that great food brings people together. Our recipes are
                                        inspired by family traditions, crafted using the freshest ingredients and cooked
                                        with love. Whether you’re here for a quick lunch, a family dinner, or a special
                                        celebration, we aim to make every meal a memorable experience.

                                        But it's not just about the food. At LAKE VIEW, we pride ourselves on creating a
                                        warm, welcoming atmosphere where you can relax, enjoy, and make lasting memories
                                        with the people who matter most. Our team is passionate about hospitality, and
                                        we’re dedicated to ensuring that every visit feels like coming home.</p>
                              </div>
                         </div>
                    </div>

                    <div class="col-md-6 col-sm-12">
                         <div class="wow fadeInUp about-image" data-wow-delay="0.6s">
                              <img src="images/about-image.jpg" class="img-responsive" alt="">
                         </div>
                    </div>

               </div>
          </div>
     </section>

     <!-- TEAM -->
     <section id="team" data-stellar-background-ratio="0.5">
          <div class="container">
               <div class="row">

                    <div class="col-md-12 col-sm-12">
                         <div class="section-title wow fadeInUp" data-wow-delay="0.1s">
                              <h2>Meet our chefs</h2>
                              <h4>They are nice &amp; friendly</h4>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-4">
                         <div class="team-thumb wow fadeInUp" data-wow-delay="0.2s">
                              <img src="images/Harpal Singh Sokhi.jpg" class="img-responsive" alt="">
                              <div class="team-hover">
                                   <div class="team-item">
                                        <h4>Duis vel lacus id magna mattis vehicula</h4>
                                        <ul class="social-icon">
                                             <li><a href="#" class="fa fa-linkedin-square"></a></li>
                                             <li><a href="#" class="fa fa-envelope-o"></a></li>
                                        </ul>
                                   </div>
                              </div>
                         </div>
                         <div class="team-info">
                              <h3>Harpal Singh Sokhi</h3>
                              <p>Kitchen Officer</p>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-4">
                         <div class="team-thumb wow fadeInUp" data-wow-delay="0.4s">
                              <img src="images/vineet Bhatia.jpg" class="img-responsive" alt="">
                              <div class="team-hover">
                                   <div class="team-item">
                                        <h4>Cras suscipit neque quis odio feugiat</h4>
                                        <ul class="social-icon">
                                             <li><a href="#" class="fa fa-instagram"></a></li>
                                             <li><a href="#" class="fa fa-flickr"></a></li>
                                        </ul>
                                   </div>
                              </div>
                         </div>
                         <div class="team-info">
                              <h3>Vineet Bhatia</h3>
                              <p>Owner &amp; Manager</p>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-4">
                         <div class="team-thumb wow fadeInUp" data-wow-delay="0.6s">
                              <img src="images/Saransh Goila.jpg" class="img-responsive" alt="">
                              <div class="team-hover">
                                   <div class="team-item">
                                        <h4>Etiam auctor enim tristique faucibus</h4>
                                        <ul class="social-icon">
                                             <li><a href="#" class="fa fa-github"></a></li>
                                             <li><a href="#" class="fa fa-google"></a></li>
                                        </ul>
                                   </div>
                              </div>
                         </div>
                         <div class="team-info">
                              <h3>Saransh Goila</h3>
                              <p>Pizza Specialist</p>
                         </div>
                    </div>

               </div>
          </div>
     </section>

     <!-- MENU-->
     <section id="menu" data-stellar-background-ratio="0.5">
          <div class="container">
               <div class="row">

                    <div class="col-md-12 col-sm-12">
                         <div class="section-title wow fadeInUp" data-wow-delay="0.1s">
                              <h2>Our Menus</h2>
                              <h4>Tea Time &amp; Dining</h4>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-6">
                         <!-- MENU THUMB -->
                         <div class="menu-thumb">
                              <a href="images/menu-image1.jpg" class="image-popup" title="American Breakfast">
                                   <img src="images/menu-image1.jpg" class="img-responsive" alt="">

                                   <div class="menu-info">
                                        <div class="menu-item">
                                             <h3>American Breakfast</h3>
                                             <p>Tomato / Eggs / Sausage</p>
                                        </div>
                                        <div class="menu-price">
                                             <span>₹2000</span>
                                        </div>
                                   </div>
                              </a>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-6">
                         <!-- MENU THUMB -->
                         <div class="menu-thumb">
                              <a href="images/menu-image2.jpg" class="image-popup" title="Self-made Salad">
                                   <img src="images/menu-image2.jpg" class="img-responsive" alt="">

                                   <div class="menu-info">
                                        <div class="menu-item">
                                             <h3>Self-made Salad</h3>
                                             <p>Green / Fruits / Healthy</p>
                                        </div>
                                        <div class="menu-price">
                                             <span>₹1800</span>
                                        </div>
                                   </div>
                              </a>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-6">
                         <!-- MENU THUMB -->
                         <div class="menu-thumb">
                              <a href="images/menu-image3.jpg" class="image-popup" title="Chinese Noodle">
                                   <img src="images/menu-image3.jpg" class="img-responsive" alt="">

                                   <div class="menu-info">
                                        <div class="menu-item">
                                             <h3>Chinese Noodle</h3>
                                             <p>Pepper / Chicken / Vegetables</p>
                                        </div>
                                        <div class="menu-price">
                                             <span>₹1500</span>
                                        </div>
                                   </div>
                              </a>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-6">
                         <!-- MENU THUMB -->
                         <div class="menu-thumb">
                              <a href="images/menu-image4.jpg" class="image-popup" title="Rice Soup">
                                   <img src="images/menu-image4.jpg" class="img-responsive" alt="">

                                   <div class="menu-info">
                                        <div class="menu-item">
                                             <h3>Rice Soup</h3>
                                             <p>Green / Chicken</p>
                                        </div>
                                        <div class="menu-price">
                                             <span>₹1000</span>
                                        </div>
                                   </div>
                              </a>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-6">
                         <!-- MENU THUMB -->
                         <div class="menu-thumb">
                              <a href="images/menu-image5.jpg" class="image-popup" title="Project title">
                                   <img src="images/menu-image5.jpg" class="img-responsive" alt="">

                                   <div class="menu-info">
                                        <div class="menu-item">
                                             <h3>Deli Burger</h3>
                                             <p>Beef / Fried Potatoes</p>
                                        </div>
                                        <div class="menu-price">
                                             <span>₹3000</span>
                                        </div>
                                   </div>
                              </a>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-6">
                         <!-- MENU THUMB -->
                         <div class="menu-thumb">
                              <a href="images/menu-image6.jpg" class="image-popup" title="Project title">
                                   <img src="images/menu-image6.jpg" class="img-responsive" alt="">

                                   <div class="menu-info">
                                        <div class="menu-item">
                                             <h3>Big Flat Fried</h3>
                                             <p>Pepper / Crispy</p>
                                        </div>
                                        <div class="menu-price">
                                             <span>₹2000</span>
                                        </div>
                                   </div>
                              </a>
                         </div>
                    </div>

                    <!-- my edit................................................................ -->


               </div>
          </div>
     </section>

     <!-- TESTIMONIAL -->
     <section id="testimonial" data-stellar-background-ratio="0.5">
          <div class="overlay"></div>
          <div class="container">
               <div class="row">

                    <div class="col-md-12 col-sm-12">
                         <div class="section-title wow fadeInUp" data-wow-delay="0.1s">
                              <h2>Reviews</h2>
                         </div>
                    </div>

                    <div class="col-md-offset-2 col-md-8 col-sm-12">
                         <div class="owl-carousel owl-theme">
                              <div class="item">
                                   <p>An integer position was in front before venenatis, while dappled positioning was
                                        arranged nicely. Maecenas' mollis intervention of the fauces, without any
                                        hindrance of the embrace.</p>
                                   <div class="tst-author">
                                        <h4>Digital Carlson</h4>
                                        <span>Quiver as much as it is.</span>
                                   </div>
                              </div>

                              <div class="item">
                                   <p>People inhabit the lands of old age and of life's struggle, and they experience
                                        hunger in the face of difficulty and challenges. The seating or vestibule is as
                                        straightforward as it is. </p>
                                   <div class="tst-author">
                                        <h4>Johnny Stephen</h4>
                                        <span>Great unless the door is a tongue</span>
                                   </div>
                              </div>

                              <div class="item">
                                   <p>Live the life where the assembly is graceful, flowing with ease and elegance. The
                                        gateway or passage of life does not just lead; it moves forward with
                                        consistency, guiding you through challenges in style.</p>
                                   <div class="tst-author">
                                        <h4>Jessie White</h4>
                                        <span>Of life, the lace/tangle of the elevated urn desires</span>
                                   </div>
                              </div>

                         </div>
                    </div>

               </div>
          </div>
     </section>

     <!-- CONTACT -->
     <section id="contact" data-stellar-background-ratio="0.5">
          <div class="container">
               <div class="row">
                    <!-- How to change your own map point
            1. Go to Google Maps
            2. Click on your location point
            3. Click "Share" and choose "Embed map" tab
            4. Copy only URL and paste it within the src="" field below
     -->
                    <div class="wow fadeInUp col-md-6 col-sm-12" data-wow-delay="0.4s">
                         <div id="google-map">
                              <iframe
                                   src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3647.3030413476204!2d100.5641230193719!3d13.757206847615207!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xf51ce6427b7918fc!2sG+Tower!5e0!3m2!1sen!2sth!4v1510722015945"
                                   allowfullscreen></iframe>
                         </div>
                    </div>

                    <div class="col-md-6 col-sm-12">

                         <div class="col-md-12 col-sm-12">
                              <div class="section-title wow fadeInUp" data-wow-delay="0.1s">
                                   <h2>Contact Us</h2>
                              </div>
                         </div>

                         <!-- CONTACT FORM -->
                         <form action="#" method="post" class="wow fadeInUp" id="contact-form" role="form"
                              data-wow-delay="0.8s">

                              <!-- IF MAIL SENT SUCCESSFUL  // connect this with custom JS -->
                              <h6 class="text-success">Your message has been sent successfully.</h6>

                              <!-- IF MAIL NOT SENT -->
                              <h6 class="text-danger">E-mail must be valid and message must be longer than 1 character.
                              </h6>

                              <div class="col-md-6 col-sm-6">
                                   <input type="text" class="form-control" id="cf-name" name="name"
                                        placeholder="Full name">
                              </div>

                              <div class="col-md-6 col-sm-6">
                                   <input type="email" class="form-control" id="cf-email" name="email"
                                        placeholder="Email address">
                              </div>

                              <div class="col-md-12 col-sm-12">
                                   <input type="text" class="form-control" id="cf-subject" name="subject"
                                        placeholder="Subject">

                                   <textarea class="form-control" rows="6" id="cf-message" name="message"
                                        placeholder="Tell about your project"></textarea>

                                   <button type="submit" class="form-control" id="cf-submit" name="submit">Send
                                        Message</button>
                              </div>
                         </form>
                    </div>

               </div>
          </div>
     </section>

     <!-- FOOTER -->
     <footer id="footer" data-stellar-background-ratio="0.5">
          <div class="container">
               <div class="row">

                    <div class="col-md-3 col-sm-8">
                         <div class="footer-info">
                              <div class="section-title">
                                   <h2 class="wow fadeInUp" data-wow-delay="0.2s">Find us</h2>
                              </div>
                              <address class="wow fadeInUp" data-wow-delay="0.4s">
                                   <p>123 nulla a cursus rhoncus,<br> augue sem viverra 10870<br>id ultricies sapien</p>
                              </address>
                         </div>
                    </div>

                    <div class="col-md-3 col-sm-8">
                         <div class="footer-info">
                              <div class="section-title">
                                   <h2 class="wow fadeInUp" data-wow-delay="0.2s">Reservation</h2>
                              </div>
                              <address class="wow fadeInUp" data-wow-delay="0.4s">
                                   <p>090-080-0650 | 090-070-0430</p>
                                   <p><a href="mailto:info@company.com">info@company.com</a></p>
                                   <p>LINE: eatery247 </p>
                              </address>
                         </div>
                    </div>

                    <div class="col-md-4 col-sm-8">
                         <div class="footer-info footer-open-hour">
                              <div class="section-title">
                                   <h2 class="wow fadeInUp" data-wow-delay="0.2s">Open Hours</h2>
                              </div>
                              <div class="wow fadeInUp" data-wow-delay="0.4s">
                                   <p>Monday: Closed</p>
                                   <div>
                                        <strong>Tuesday to Friday</strong>
                                        <p>7:00 AM - 9:00 PM</p>
                                   </div>
                                   <div>
                                        <strong>Saturday - Sunday</strong>
                                        <p>11:00 AM - 10:00 PM</p>
                                   </div>
                              </div>
                         </div>
                    </div>

                    <div class="col-md-2 col-sm-4">
                         <ul class="wow fadeInUp social-icon" data-wow-delay="0.4s">
                              <li><a href="#" class="fa fa-facebook-square" attr="facebook icon"></a></li>
                              <li><a href="#" class="fa fa-twitter"></a></li>
                              <li><a href="#" class="fa fa-instagram"></a></li>
                              <li><a href="#" class="fa fa-google"></a></li>
                         </ul>

                         <div class="wow fadeInUp copyright-text" data-wow-delay="0.8s">
                              <p><br>Copyright &copy; 2018 <br>Your Company Name

                                   <br><br>Design: TemplateMo
                              </p>
                         </div>
                    </div>

               </div>
          </div>
     </footer>

     <!-- SCRIPTS -->
     <script src="js/jquery.js"></script>
     <script src="js/bootstrap.min.js"></script>
     <script src="js/jquery.stellar.min.js"></script>
     <script src="js/wow.min.js"></script>
     <script src="js/owl.carousel.min.js"></script>
     <script src="js/jquery.magnific-popup.min.js"></script>
     <script src="js/smoothscroll.js"></script>
     <script src="js/custom.js"></script>

</body>

</html>











 

 

 

 

 

 

 

CONCLUSION

Deploying a static restaurant website using Azure Services offers an efficient, scalable, and cost-effective solution for establishing a robust online presence. By leveraging Azure Blob Storage for hosting, Azure CDN for fast, global content delivery, and Azure DNS for domain management, the website achieves high performance, reliability, and accessibility. This approach minimizes the need for ongoing infrastructure maintenance while ensuring the website can handle increased traffic and provide a seamless user experience. Overall, Azure provides a flexible and secure platform, allowing the restaurant to focus on growing its business while ensuring an optimal digital presence.


