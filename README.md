sdkFacade.presentPayment(at: self, paymentOptions: paymentOptions) { (result) in
   print("ECommPay SDK finished with status \\(result.status.rawValue)")
   ...
 }#import <ecommpaySDK/ECommPayhostsSDK.h>viewDidLoad
 EcommpaySDK *sdkFacade = [[EcommpaySDK alloc] init];
 PaymentOptions *paymen
 
 [sdkFacade presentPaymentAt:self paymentOptions:paymentOptions 
     completionHandler:^(PaymentResult *result) {
     NSLog(@"ECommPay SDK finished with status %ld", (long)result.status);
     ...
 }];
