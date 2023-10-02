# PicsumDemo
Code Samples for SUGCON 2023 talk

## Instructions

1. Create a free account on Pipedream.com.
2. Create a project and workflow. Initate the workflow with a Webhook action: 
![image](https://github.com/dsolovay/PicsumDemo/assets/689532/98a68cf1-f78b-47cc-88d9-d250cee2db12)
3. Create steps for each JS file in `steps` folder, removing `.js` prefix.  Steps must be in this order:
  1. configure
  2. get_parameters
  3. Save_picsum_image
  4. Get_photo_url
  5. Refresh_auth_code
  6. Get_meedia_upload_url
  7. post_images_to_sitecore
  8. update_image_link_and_workflow_state
9. Create a Docker 10.3.1 XM or XP environment. Enable bearer token generation by adding resources in `docker` folder:
  1. Postman endpoint configuration
  2. Docker compose override file
10. Install package in `package` folder to create templates, workflow, and required content roots.
11. Get a free account on NGrok.
12. Enable NGrok configuration (TODO find link)
13. Set up service endpionts for "cm" and "id" services.
14. Load scripts in `scripts` folder in a PowerShell sessoin.
15. Run `Set-NgrokIps`
16. Run `Start-NgrokTunnels`
17. Create settings in Pipedream.com (path):
  1.  TODO
19. Feature should now be working. Create an item as an author under Sitecore\Content\Picsum Demo, and execute the "Submit to Picsum" workflow command. This should trigger the workflow execution on Pipedraam, and an image to be uploaed to the media library and set in the Image field.
     



