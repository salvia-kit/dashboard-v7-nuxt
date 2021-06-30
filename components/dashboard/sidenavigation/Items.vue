<template>
  <div>
    <sidenav-items-section name="Applications">
      <sidenav-item title="Users" to="/">
        <users-icon />
      </sidenav-item>
      <sidenav-item title="Medias" to="/admin/medias">
        <medias-icon />
      </sidenav-item>
      <sidenav-item title="Contacts" to="/admin/contacts">
        <contact-icon />
      </sidenav-item>
    </sidenav-items-section>

    <sidenav-items-section name="Monitoring">
      <sidenav-item title="Terminal" to="/admin/terminal">
        <terminal-icon />
      </sidenav-item>
      <sidenav-item title="Recycle Bin" to="/admin/recycle-bin">
        <recycle-bin-icon />
      </sidenav-item>
      <sidenav-item title="Servers" to="/admin/servers">
        <servers-icon />
      </sidenav-item>
    </sidenav-items-section>

    <sidenav-items-section name="Guides">
      <sidenav-item title="Documentation" to="/admin/documentation">
        <documentation-icon />
      </sidenav-item>
    </sidenav-items-section>
  </div>
</template>

<script>
import SidenavItem from './Item.vue';
import SidenavItemsSection from './Section.vue';

/* ICONS */
import UsersIcon from './icons/Users.vue';
import MediasIcon from './icons/Medias.vue';
import ContactIcon from './icons/Contact.vue';
import ServersIcon from './icons/Servers.vue';
import TerminalIcon from './icons/Terminal.vue';
import RecycleBinIcon from './icons/RecycleBin.vue';
import DocumentationIcon from './icons/Documentation.vue';

export default {
  name: 'SidenavItems',
  components: {
    UsersIcon,
    MediasIcon,
    SidenavItem,
    ContactIcon,
    ServersIcon,
    TerminalIcon,
    RecycleBinIcon,
    DocumentationIcon,
    SidenavItemsSection,
  },
};
</script>
