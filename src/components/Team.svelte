<script>
  import TeamMember from './TeamMember.svelte';
  const teamMembers = [
    {
      img: '/team/elias.jpg',
      fullName: 'Elias Tazartes',
      role: 'CEO & Co-Founder',
      twitterHandle: 'etazou',
    },
    {
      img: '/team/clement.jpeg',
      fullName: 'Clement Walter',
      role: 'CTO & Co-Founder',
      twitterHandle: 'clementwalter',
    },
    {
      img: '/team/danilo.jpeg',
      fullName: 'Danilo Kim',
      role: 'Ecosystem & Co-Founder',
      twitterHandle: 'danilowhk2',
    },
    {
      img: '/team/abdel.jpeg',
      fullName: 'Abdelhamid Bakhta',
      role: 'Tech Advisor',
      twitterHandle: 'dimahledba',
    },
    {
      img: '/team/mentor.jpeg',
      fullName: 'Mentor Reka',
      role: 'Financial Advisor',
      twitterHandle: 'mentornotpseudo',
    },
    {
      img: '/team/greg.jpeg',
      fullName: 'Gregory Edison',
      role: 'Core Dev',
      twitterHandle: 'greged93',
    },
    {
      img: '/team/johann.jpeg',
      fullName: 'Johann Bestowrous',
      role: 'Core Dev',
      twitterHandle: 'opinionsonline',
    },
  ];
</script>

<div
  class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-3 md:gap-6 lg:gap-8"
>
  {#each teamMembers as member}
    <TeamMember
      img={member.img}
      fullName={member.fullName}
      role={member.role}
      twitterHandle={member.twitterHandle}
    />
  {/each}
</div>
