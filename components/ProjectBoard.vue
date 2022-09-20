<template>
<div>
    <div class="bg-gray-200 text-center font-normal text-6xl pt-10 pb-4 ">
      My Work
    </div>
    <div class="bg-gray-200 min-h-full px-2 flex flex-wrap pb-8 justify-center">
      <div v-for="(project, index) in projects" v-bind:key="(project, index)">
          <ProjectCard :doc="project"/>
      </div>
    </div>
</div>
</template>

<script>
import ProjectCard from './ProjectCard'

export default {
    components: {
        ProjectCard,
    },
    data: () => ({
    projects: [
      {
          imageURL: 'https://images.unsplash.com/photo-1522659333390-223b26e7bb00?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80',
          title: 'Drivers Licence Barcode Scanner',
          content: 'A OpenCV project that extracts information from a drivers licence with a photo of the back.',
          tags : [
            {name: 'Read Blog', link:'../blog/opencv-update'},
            {name: 'Source Code', link:'https://github.com/orionnelson/DlicenceZxingParse'}
          ]
      },
      {
          imageURL: 'https://images.unsplash.com/photo-1472851294608-062f824d29cc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1300&q=80',
          title: 'Shop Unicorn Webstore',
          content: 'A Webstore Template with a Rating and Review system',
          tags: [
            {name: 'Source Code', link: 'https://github.com/sidoverflow/shopunicorn'},
            {name: 'Live Link', link: 'https://unicorn.or9.ca'},
          ],
      },
      {
          imageURL: 'https://images.unsplash.com/photo-1597733336794-12d05021d510?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80',
          title: 'Web Requests Scripts',
          content: 'Find Source Code for Google2Link, Abstractive Predictions and other needs.',
          tags: [
            {name: 'Source Code', link: 'https://github.com/orionnelson/requests-practice'},
            {name: 'Har2Requests', link: 'https://github.com/louisabraham/har2requests'},
            {name: 'Download', link: 'https://github.com/orionnelson/requests-practice/releases/'},
          ],
      },
      {
          imageURL: 'https://images.unsplash.com/photo-1640552435388-a54879e72b28?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80',
          title: 'Linux Tutorials',
          content: "Here's the fix for these issues",
          tags: [
            {name: 'Overwritten Grub EFI', link: '../blog/opencv-update'},
          ],
      },
      {
          imageURL: 'https://or9.ca/images/hdesk.jpg',
          title: 'Help Desk Application',
          content: 'A Socket based Support app for helping anonymous clients.',
          tags: [
            {name: 'Source Code', link: 'https://github.com/ReubenMathew/HelpDesk'},
            {name: 'Live Link', link: 'https://help-desk-psi.vercel.app/'},
          ],
      },
      {
          imageURL: 'https://images.unsplash.com/photo-1533158307587-828f0a76ef46?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80',
          title: 'FFMPEG Batch Folder Resizer',
          content: 'An application to prevent you from uploading your photos to random sites and keeps folder hiarchy.' ,
          tags: [
            {name: 'Source Code', link: 'https://github.com/orionnelson/ffmpeg-resizer'},
            {name: 'Demo', link: 'https://youtu.be/a2mhB3tGfLU'},
            {name: 'Download', link: 'https://github.com/orionnelson/ffmpeg-resizer/releases'},
          ],
      },
      {
          imageURL: 'https://images.unsplash.com/photo-1606511554594-80a9be4240ca?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80',
          title: 'Wizlight Controller Api',
          content: 'Connect and Control Multiple Wizlights by Socket or Wireshark HID.',
          tags: [
            {name: 'Source Code', link: 'https://github.com/orionnelson/Wizligt-Socket-HID'},
          ],
      },
      {
          imageURL: 'https://or9.ca/images/srgb.jpg',
          title: 'SignalRGB AW558 Mouse Plugin',
          content: 'A SignalRGB plugin made from reverse engineering HID protocols with Wireshark.',
          tags: [
            {name: 'Source Code', link: 'https://github.com/orionnelson/AW558-SignalPlugin'},
          ],
      },
      {
          imageURL: 'https://images.unsplash.com/photo-1523726491678-bf852e717f6a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80',
          title: 'Software Design Projects',
          content: 'A Collection of various software design projects.',
          tags: [
            {name: 'Unit Converter', link: 'https://github.com/orionnelson/lab6'},
            {name: 'Javadoc Example', link: 'https://or9.ca/Lab6/'},
            {name: 'Soccer App', link: 'https://github.com/orionnelson/football-game'},
            {name: 'Shape Sorter App', link: 'https://github.com/orionnelson/labw3'},
          ],
      },

    ]
  })
}
</script>
