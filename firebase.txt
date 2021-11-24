// Import the functions you need from the SDKs you need
import firebase from 'firebase/compat/app';
import 'firebase/compat/auth'
// TODO: Add SDKs for Firebase products that you want to use
// https://firebase.google.com/docs/web/setup#available-libraries

// Your web app's Firebase configuration
const firebaseConfig = {
  apiKey: "AIzaSyCzlijnmIj8CN3l2vIbOBf2VjTaEXzJC9s",
  authDomain: "fir-auth-5d929.firebaseapp.com",
  projectId: "fir-auth-5d929",
  storageBucket: "fir-auth-5d929.appspot.com",
  messagingSenderId: "186238636359",
  appId: "1:186238636359:web:992006b255d571b37e7c62"
};

let app;
if(firebaseConfig.apps.length === 0)
{
    app = firebase.initializeApp(firebaseConfig);
}else{
    app = firebase.app()
}
// Initialize Firebase
const auth = firebase.auth()

export {auth};