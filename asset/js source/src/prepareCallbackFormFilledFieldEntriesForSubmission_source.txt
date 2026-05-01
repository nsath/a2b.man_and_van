         <script type="text/javascript">

          function prepareCallbackFormFilledFieldEntriesForSubmission (  ) {

            var customer_name = $ ( "input [name = contact-name-whom-to-call ]" ) .val (  ) ;

            var customer_number = $ ( "input [name = contact-number-to-call ]" ) .val (  ) ;

            $ .ajax ( {

              type: "POST",

              url: "mailer.php",

              dataType: "text",

              encode: true,

              data:

                "customername=" + customer_name +

                "&phonecontactNumber=" + customer_number,

              success: function (  ) {

                

              } ,

              error: function (  ) {

                

              } ,

            } ) ;

          }

         </script>