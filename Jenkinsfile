// @Library('my-shared-library') _

// pipeline{

//     agent any

//     parameters{
//         choice(name: 'action', choices: 'Create\nDestroy', description: "Choose Create/Destroy" )
//     }

//     stages{

//         stage('Git Checkout'){
//         when { expression { params.action == 'Create' } }

//             steps{
//             gitCheckout(
//                 branch: "main",
//                 url: "https://github.com/abdulmalik-devs/my_java_app.git"
//             )
//             }
//         }
//         stage('Unit Test Maven'){
//         when { expression { params.action == 'Create' } }

//             steps{
//                 script{
                    
//                     mvnTest()
//                 }
//             }
//         }
//         stage('Integration Test Maven'){
//         when { expression { params.action == 'Create' } }

//             steps{
//                 script{
                    
//                     mvnIntegrationTest()
//                 }
//             }
//         }
//     }
// }